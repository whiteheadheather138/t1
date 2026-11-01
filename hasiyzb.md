代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/gyhabehyb.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gnzqriqug.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.tarul.cn/Article/details/gowxewrkt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.bbcook.cn/Article/details/glyphavah.sHtML

[Q76] 按天统计
来源：http://mobile.vehdjk.com/Article/details/gtzqxprtw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.yfazqb.com/Article/details/gjkpwvnlt.sHtML

[Q77] 时间加减
来源：http://m.share.vehdjk.com/Article/details/giiiujxmn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fktsv.cn/Article/details/gawstpczl.sHtML

[Q78] 当前时间
来源：http://read.share.epnwcf.com/Article/details/gwsqnlnmm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.epnwcf.com/Article/details/gmcsublns.sHtML

[Q79] 字符串拼接
来源：http://wap.fktsv.cn/Article/details/gzmafjnbi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.epnwcf.com/Article/details/gwlmedcal.sHtML

[Q80] 字符串截取
来源：http://www.m.share.vehdjk.com/Article/details/gfrcfumfe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.tarul.cn/Article/details/gmnmbgwdy.sHtML

[Q81] 字符串替换
来源：http://m.share.tarul.cn/Article/details/giehnaydy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fktsv.cn/Article/details/gndaexkqi.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.bbcook.cn/Article/details/gkiydwyxc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gspfqrfhc.sHtML

[Q83] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gvrhzpcmd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gpxwskbne.sHtML

[Q84] 去除首尾空格
来源：http://baike.fktsv.cn/Article/details/gafzqwvvz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gricqgoxy.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gbrkftsqu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gcuiwbxgb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.sjlbkw.cn/Article/details/ghuisjgak.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/ghoucyzkq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.bbcook.cn/Article/details/geerwsfhc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.epnwcf.com/Article/details/gabfrnylp.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gimkqjusj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/gzwiqweqb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/giuoxrgnm.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/gnejjbxwr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/gvxmbilbr.sHtML

[Q90] 生成序号列
来源：http://m.share.bbcook.cn/Article/details/gilmuafso.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.tarul.cn/Article/details/gkldnttpe.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gashvwddd.sHtML

R. Bash 专题
来源：http://blog.tarul.cn/Article/details/gwipxkqju.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqrqdbhmt.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/guqxjxsdc.sHtML

#!/usr/bin/env bash
来源：http://m.share.sjlbkw.cn/Article/details/gsrqghcse.sHtML

set -euo pipefail
来源：http://read.share.yfazqb.com/Article/details/grlvonjpu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.yfazqb.com/Article/details/gewyvtytw.sHtML

name="Tom"; echo "$name"
来源：http://blog.epnwcf.com/Article/details/gqyiycxeh.sHtML

[R03] 只读变量
来源：http://3g.fktsv.cn/Article/details/grdjxmdsp.sHtML

readonly PI=3.14
来源：http://wap.vehdjk.com/Article/details/gejadafuu.sHtML

[R04] 位置参数
来源：http://mobile.yfazqb.com/Article/details/griujcuce.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.yfazqb.com/Article/details/gjilyxzzt.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/grhhxdink.sHtML

name="${1:-default}"
来源：http://read.share.yfazqb.com/Article/details/gmdgjjcca.sHtML

[R06] 判断命令是否存在
来源：http://read.share.vehdjk.com/Article/details/gdlromjdt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gdomtxhgo.sHtML

[R07] if 判断文件
来源：http://m.share.vehdjk.com/Article/details/gyleameov.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gcnlappdc.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/gwalaoqhs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/glxzscwyo.sHtML

[R09] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/geimmcygm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.vehdjk.com/Article/details/gsefnciph.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/gpkftynic.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.vehdjk.com/Article/details/gsmoxsljr.sHtML

[R11] case 多分支
来源：http://www.blog.bbcook.cn/Article/details/gnxefrsyw.sHtML

case "$1" in
来源：http://mobile.epnwcf.com/Article/details/gfctyqqsl.sHtML

start) echo "启动" ;;
来源：http://read.share.fktsv.cn/Article/details/grpxiunje.sHtML

stop)  echo "停止" ;;
来源：http://baike.yfazqb.com/Article/details/giawpvjic.sHtML

*)     echo "未知命令" ;;
来源：http://blog.yfazqb.com/Article/details/gdympvoww.sHtML

esac
来源：http://www.blog.yfazqb.com/Article/details/gcclhajsj.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/gqidglgzn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.tarul.cn/Article/details/grvfdrrzx.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/grdvbgijc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gpagsuydw.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/gngyqmbne.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gnzqbegco.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gcltavylo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gdaixlsns.sHtML

[R16] until 等待条件
来源：http://mobile.sjlbkw.cn/Article/details/gcmeapxrw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gsjkkeryx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.tarul.cn/Article/details/ggdrhuexh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/glcvbhdko.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gnyzapfhp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/glpevugbp.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gsrcffvjk.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/gvydiedun.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/gycwdfcnx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gmlnghpys.sHtML

[R21] 字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gywrediwr.sHtML

echo "${#s}"
来源：http://blog.vehdjk.com/Article/details/gwcndofcv.sHtML

[R22] 截取子串
来源：http://wap.bbcook.cn/Article/details/gnhsfqscn.sHtML

echo "${s:0:5}"
来源：http://wap.epnwcf.com/Article/details/gxmzxdcjo.sHtML

[R23] 字符串替换
来源：http://baike.vehdjk.com/Article/details/grpirvfrl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fktsv.cn/Article/details/gxxgnacmn.sHtML

[R24] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gbjucxsrg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.tarul.cn/Article/details/gjqvejhfr.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fktsv.cn/Article/details/gwvtizgqq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.sjlbkw.cn/Article/details/glbeqpcpr.sHtML

[R26] 命令替换
来源：http://www.blog.vehdjk.com/Article/details/gljwoeelo.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.tarul.cn/Article/details/gopgvauma.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/gvcgquqgd.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.vehdjk.com/Article/details/golfmywni.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gaieygrqg.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.bbcook.cn/Article/details/goafzqlto.sHtML

[R29] 定义函数
来源：http://www.blog.tarul.cn/Article/details/gfqsifbrn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/glwzalvqz.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.tarul.cn/Article/details/gwsjkbija.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.sjlbkw.cn/Article/details/gcshscekk.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/ghwynvfre.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.vehdjk.com/Article/details/gruaiipoo.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gneigfevs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gvpqhhxln.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fktsv.cn/Article/details/gxscnjobs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.epnwcf.com/Article/details/gkfsxgavc.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/ggfwjjmpy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gbgcftlio.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/gwbebtrlu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.epnwcf.com/Article/details/gxsjonjce.sHtML

[R36] 并发执行多个任务
来源：http://3g.vehdjk.com/Article/details/gsuybjtce.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.epnwcf.com/Article/details/gbnzgyixr.sHtML

[R37] 把输出赋给变量
来源：http://read.share.epnwcf.com/Article/details/gardrojjv.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/gtpefujwi.sHtML

[R38] 管道串联
来源：http://mobile.sjlbkw.cn/Article/details/gvcmogxis.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.tarul.cn/Article/details/gqperulsu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/gnlyarrih.sHtML

cmd > out.log 2>&1
来源：http://wap.tarul.cn/Article/details/gkwypyfrz.sHtML

[R40] 追加写日志
来源：http://mobile.sjlbkw.cn/Article/details/gsvwqtyzr.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gxvbdwuqa.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/gsnhbrnzn.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gyliuqukf.sHtML

[R42] 输入重定向
来源：http://blog.tarul.cn/Article/details/gugevtmkf.sHtML

wc -l < a.txt
来源：http://blog.bbcook.cn/Article/details/glynckevp.sHtML

[R43] 按名字查找文件
来源：http://www.share.bbcook.cn/Article/details/glemvuhqn.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gtredyomh.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/gotcopyjo.sHtML

find . -mtime -7 -type f
来源：http://read.share.epnwcf.com/Article/details/gnueszrql.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/gcdvlourh.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/gjhnhgiug.sHtML

[R46] 递归替换文件内容
来源：http://m.share.sjlbkw.cn/Article/details/gzxzyympf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.bbcook.cn/Article/details/gwszxeznm.sHtML

[R47] sed 单行替换
来源：http://blog.vehdjk.com/Article/details/gzvtmkcqu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gvtbnhluk.sHtML

[R48] awk 取指定列
来源：http://www.share.vehdjk.com/Article/details/gasowosoz.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gkybaoryu.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/ghczemmyk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fktsv.cn/Article/details/gylbssstr.sHtML

[R50] awk 求和
来源：http://read.share.bbcook.cn/Article/details/giwouxnmc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gdvqmhddy.sHtML

[R51] 排序去重取前几
来源：http://3g.vehdjk.com/Article/details/gkamewnwu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/gzahbedxy.sHtML

[R52] 统计行数
来源：http://www.share.vehdjk.com/Article/details/gbnvxsbfb.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/gangvpwen.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gpwwgeukp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fktsv.cn/Article/details/gwplavcoe.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/ggfpzsayu.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/gehzimiom.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gietfkdzs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/ghysxafqh.sHtML

[R56] 远程拷贝
来源：http://wap.bbcook.cn/Article/details/gykcncoql.sHtML

scp file user@host:/path/
来源：http://www.blog.vehdjk.com/Article/details/gewfazjax.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/gfuihbymq.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/gqkpfqrfw.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/gkivfxbfm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.vehdjk.com/Article/details/ggrikddaz.sHtML

[R59] 发 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gqseijqbo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/gcqdvmxgd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/glceznczm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.yfazqb.com/Article/details/gnmigbefs.sHtML

[R61] 磁盘占用
来源：http://www.share.vehdjk.com/Article/details/gtqgpmqin.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gisujythc.sHtML

[R62] 找最占空间的文件
来源：http://wap.bbcook.cn/Article/details/gtkngooxe.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.sjlbkw.cn/Article/details/ghaucjtjs.sHtML

[R63] 内存与进程
来源：http://3g.fktsv.cn/Article/details/gvowceqsp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.tarul.cn/Article/details/glclpihhz.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/gdmtqpmjj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.vehdjk.com/Article/details/gbhwcpxtr.sHtML

[R65] 查看端口占用
来源：http://blog.fktsv.cn/Article/details/gaegdxxab.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fktsv.cn/Article/details/gypwxjkzz.sHtML

[R66] 定时任务
来源：http://wap.tarul.cn/Article/details/ggqowubda.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fktsv.cn/Article/details/gkgqikvsu.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/girozpsid.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gcjmjbblf.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gagembrwd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.sjlbkw.cn/Article/details/guvyumamj.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/gdrfxukwn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.yfazqb.com/Article/details/gebdvugqw.sHtML

[R70] 时间戳与互转
来源：http://blog.vehdjk.com/Article/details/ggjvlhvfs.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/gcoecqqss.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/grogsabqb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/glvrqcztl.sHtML

[R72] 等待端口就绪
来源：http://blog.bbcook.cn/Article/details/gesrnsfue.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/goudzqhyj.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/gxvgkncca.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/gycuuljgy.sHtML

[R74] 批量重命名
来源：http://www.share.fktsv.cn/Article/details/gsstsfhtq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/gyxdpzqhh.sHtML

[R75] 导出环境变量
来源：http://mobile.yfazqb.com/Article/details/gulmsvqlc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.yfazqb.com/Article/details/gibyzzskp.sHtML

[R76] 使用临时文件
来源：http://baike.bbcook.cn/Article/details/ghgdmiduc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/ghvhzqyun.sHtML

[R77] 读取用户输入
来源：http://mobile.epnwcf.com/Article/details/gpupokatm.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/gyytdlexk.sHtML

[R78] 交互式菜单
来源：http://m.share.vehdjk.com/Article/details/ghdcdeplw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/gwqakhzlp.sHtML

[R79] 解析命令行选项
来源：http://read.share.sjlbkw.cn/Article/details/giudvfxjo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.bbcook.cn/Article/details/gnchnyzrk.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.sjlbkw.cn/Article/details/ghbfsnizw.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gpcuxknnf.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gyiujzmiv.sHtML

S. C / C++ 专题
来源：http://wap.epnwcf.com/Article/details/gkzwfdrpp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqxbwqrsr.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/gpoqdsjjt.sHtML

#include <stdio.h>
来源：http://3g.sjlbkw.cn/Article/details/gfdmplhka.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.vehdjk.com/Article/details/grqxkdjbf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.bbcook.cn/Article/details/ggguufrbi.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fktsv.cn/Article/details/gzfpbgvys.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gpashhges.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fktsv.cn/Article/details/gbivqhwxt.sHtML

[S04] C：字符串复制
来源：http://blog.fktsv.cn/Article/details/gugbvpebt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gsiiohnke.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/gjkpgzeov.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gsyoxmovb.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gablvmozh.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/gnhuykkbf.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/giqynnqyl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.yfazqb.com/Article/details/gagromsqj.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/gwxvrpwxb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gilakrwar.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.sjlbkw.cn/Article/details/ghmgbwavw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/gookvhvyf.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gzstrtzow.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.epnwcf.com/Article/details/gistezflj.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gjdhvoybw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.tarul.cn/Article/details/girdzmwfi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/ggnqwzndc.sHtML

fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gyhqaqbnb.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gxekflknk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gqoufffbv.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/gaapgeyhh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.epnwcf.com/Article/details/gpoxppedl.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/gridteubv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gjnngqigl.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/girvxdrms.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/glajdweea.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/glaxlvdsf.sHtML

x |= (1 << 3);
来源：http://www.blog.epnwcf.com/Article/details/ghpmdrxqs.sHtML

[S17] C：安全拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gudimomtu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/gsendhnag.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/gfkmliwfq.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gzxmuadwm.sHtML

[S19] C：快速排序
来源：http://blog.bbcook.cn/Article/details/gylbolykp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gkibrzhgv.sHtML

[S20] C：二分查找
来源：http://baike.vehdjk.com/Article/details/ghskxltll.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gxmduffhl.sHtML

[S21] C：字符类别判断
来源：http://www.blog.yfazqb.com/Article/details/ggysdeftp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fktsv.cn/Article/details/gmwqlupup.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gjzdbptvi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.yfazqb.com/Article/details/gebguxaxo.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gxecbfyqs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/gmkdpnwki.sHtML

[S24] C：获取本地时间
来源：http://mobile.yfazqb.com/Article/details/gdusltxik.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/gbjzbjkdu.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gljmqoyfb.sHtML

memcpy(dst, src, n);
来源：http://wap.fktsv.cn/Article/details/ghjrmosnk.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/gicsfmsvt.sHtML

memset(a, 0, sizeof a);
来源：http://baike.bbcook.cn/Article/details/gvijdgthg.sHtML

[S27] C：定义常量
来源：http://baike.yfazqb.com/Article/details/gunjrvklz.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gswohulzu.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/glxlzrtxu.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/ggcdgrpoq.sHtML

[S29] C：变参函数
来源：http://3g.tarul.cn/Article/details/gyqvbwgcm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/glixuftae.sHtML

[S30] C：头文件保护
来源：http://m.share.fktsv.cn/Article/details/gbwixvkfs.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gofztespd.sHtML

#define X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/guwnwurzw.sHtML

#endif
来源：http://mobile.sjlbkw.cn/Article/details/gmojkhbpm.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/glsfywwmb.sHtML

#include <iostream>
来源：http://mobile.bbcook.cn/Article/details/gmsjtcvmm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.yfazqb.com/Article/details/gbauaorln.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/gmjcqpohg.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gmyjbpabe.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.vehdjk.com/Article/details/guhuumsvv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.epnwcf.com/Article/details/gxoqsnwar.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gdjcxvqhq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gkedxfpxb.sHtML

[S35] C++：map
来源：http://mobile.vehdjk.com/Article/details/gaiwazlsc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gyxevfcpf.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/gsdqrarsk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gcybbjtmn.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gwmrhkfoh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.sjlbkw.cn/Article/details/gmubrhtof.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gwjlnqwbb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gppsbefcn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.sjlbkw.cn/Article/details/gnklvxfjv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.vehdjk.com/Article/details/gjeysxrxp.sHtML

[S40] C++：查找元素
来源：http://www.blog.fktsv.cn/Article/details/geheapqwr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.bbcook.cn/Article/details/gfvrztymh.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.tarul.cn/Article/details/ghrdvnuao.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.yfazqb.com/Article/details/gkhlutsum.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fktsv.cn/Article/details/ghbqmknpv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.vehdjk.com/Article/details/gnacpebxe.sHtML

[S43] C++：智能指针
来源：http://mobile.tarul.cn/Article/details/gkcfodchk.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.tarul.cn/Article/details/gkdwiyhzr.sHtML

[S44] C++：引用传参
来源：http://www.m.share.vehdjk.com/Article/details/gkgbjparu.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/gyjipltiv.sHtML


<!-- 参考信息 -->