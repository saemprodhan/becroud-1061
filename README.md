# becroud-1061
even time
start_day = int(input().split()[1])
start_time = list(map(int,input().split(" : ")))
end_day = int(input().split()[1])
end_time = list(map(int,input().split(" : ")))
start_second = start_day*86400+start_time[0]*3600+start_time[1]*60+start_time[2]
end_second = end_day*86400+end_time[0]*3600+end_time[1]*60+end_time[2]
total_time = end_second - start_second
day = total_time//86400
duratio = total_time%86400
hour = duratio//3600
dur = duratio%3600
minute =  dur//60
sec = dur % 60
print(f"{day} dia(s)")
print(f"{hour} hora(s)")
print(f"{minute} minuto(s)")
print(f"{sec} segundo(s)")
