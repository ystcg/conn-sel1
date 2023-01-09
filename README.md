import mysql.connector as m
conn=m.connect(host='localhost',user='root',password='admin',database="school")
cur=conn.cursor()
cur.execute('select subject, code from exam;')
for row in cur:
    S, c=row
    print(s,'(',c,')',sep=")
conn.close()
