代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.epnwcf.com/Article/details/govzkpnty.sHtML

[Q75] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gbmpdphbf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gxspmmhsz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fktsv.cn/Article/details/gpjebhjkn.sHtML

[Q76] 按天统计
来源：http://wap.epnwcf.com/Article/details/gdikgngyf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/gkjrqinrl.sHtML

[Q77] 时间加减
来源：http://mobile.sjlbkw.cn/Article/details/gqsneivmv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gqvdehgpc.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gwemvbcgp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fktsv.cn/Article/details/gmbnzdwdq.sHtML

[Q79] 字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gjfdpgpnu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.tarul.cn/Article/details/garlemmta.sHtML

[Q80] 字符串截取
来源：http://read.share.vehdjk.com/Article/details/gssxgpzbs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/gbnezjmvk.sHtML

[Q81] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/ghtouttrh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gmsyfrlpz.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.sjlbkw.cn/Article/details/gjaazfzaz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gplcjfbaj.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/guvspwfri.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gcwjvqgyq.sHtML

[Q84] 去除首尾空格
来源：http://blog.fktsv.cn/Article/details/gyftwervh.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gdezwhbum.sHtML

[Q85] 数值取整
来源：http://wap.fktsv.cn/Article/details/gbnauihag.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.bbcook.cn/Article/details/gdpaxhakj.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/gojedkxna.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.bbcook.cn/Article/details/gcofdilbn.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/gkydmmptt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/gyjmnrfmo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.tarul.cn/Article/details/gbiyotdkk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fktsv.cn/Article/details/gmzaqrqgb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.vehdjk.com/Article/details/ghuinbwya.sHtML

[Q89] 判断表是否存在
来源：http://read.share.epnwcf.com/Article/details/gylbcnnvn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.yfazqb.com/Article/details/gurjdnani.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/gtdddanpi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fktsv.cn/Article/details/gjfesxhlb.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghdsprhfm.sHtML

R. Bash 专题
来源：http://www.share.tarul.cn/Article/details/gsxaapoqd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/giweeuzyc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.bbcook.cn/Article/details/gjvlvlzeb.sHtML

#!/usr/bin/env bash
来源：http://blog.sjlbkw.cn/Article/details/grqogoyha.sHtML

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/gxbwfmxnz.sHtML

[R02] 变量赋值与使用
来源：http://mobile.yfazqb.com/Article/details/gscevvaou.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/grbjmxvgh.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/ggwqcniyv.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gzophdxmv.sHtML

[R04] 位置参数
来源：http://www.m.share.epnwcf.com/Article/details/gtzkrcmjh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.sjlbkw.cn/Article/details/gcmkdolnq.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gotuzwgjd.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/gxojzdsdp.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fktsv.cn/Article/details/gknqgrhru.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gjrpsoyzv.sHtML

[R07] if 判断文件
来源：http://www.m.share.fktsv.cn/Article/details/gvbdpjahy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.tarul.cn/Article/details/gxkgwvatc.sHtML

[R08] 数值比较
来源：http://baike.epnwcf.com/Article/details/gtrgvpuzz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gubqqzmgd.sHtML

[R09] 字符串比较
来源：http://wap.bbcook.cn/Article/details/giolpwaki.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/gulgjorzx.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/grshuncyr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.tarul.cn/Article/details/gghwrtavw.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/getviqlub.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/gbnsyvnzq.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gkkrpqjkl.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/gkyjucdgk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.vehdjk.com/Article/details/gzzoafacy.sHtML

esac
来源：http://wap.yfazqb.com/Article/details/gotlwtdbp.sHtML

[R12] for 遍历文件
来源：http://3g.tarul.cn/Article/details/gwefeqeos.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.yfazqb.com/Article/details/gryrgaitu.sHtML

[R13] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/ghffrsxhq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gpancgrzc.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gwuhogcvd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gaabipnft.sHtML

[R15] while 逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gxkttxqep.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.yfazqb.com/Article/details/gxhycgyac.sHtML

[R16] until 等待条件
来源：http://wap.vehdjk.com/Article/details/gpikulekr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gedpczkvg.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.yfazqb.com/Article/details/guiqbolqx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.vehdjk.com/Article/details/gtpgprupl.sHtML

[R18] 遍历数组
来源：http://www.m.share.tarul.cn/Article/details/ghtjcpxop.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/gxwilmgmy.sHtML

[R19] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gkhrswmrl.sHtML

echo "${#arr[@]}"
来源：http://www.share.epnwcf.com/Article/details/ggapkyseh.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gdxlkveyl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gvajrsahu.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gyewfobta.sHtML

echo "${#s}"
来源：http://www.share.epnwcf.com/Article/details/gndytfkqk.sHtML

[R22] 截取子串
来源：http://blog.fktsv.cn/Article/details/gzjyvhdia.sHtML

echo "${s:0:5}"
来源：http://www.m.share.bbcook.cn/Article/details/ghpbcmxci.sHtML

[R23] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gzplrxkme.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.tarul.cn/Article/details/gmczqsojf.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gyzyrgjns.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.sjlbkw.cn/Article/details/gonmxhsvj.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gqyvxxdmo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/gudngndoy.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gajipmejv.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fktsv.cn/Article/details/gigsflvrn.sHtML

[R27] 算术展开
来源：http://blog.epnwcf.com/Article/details/gefbdrijc.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/gjvrpmxbf.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/gdlgfahzi.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gpxmqnucx.sHtML

[R29] 定义函数
来源：http://3g.yfazqb.com/Article/details/gayptrbfn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/gggvvbvxn.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/gvzxslzuj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.tarul.cn/Article/details/gzwcnosjb.sHtML

[R31] 局部变量
来源：http://www.share.fktsv.cn/Article/details/gmxtkbkdj.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.epnwcf.com/Article/details/gruyujiss.sHtML

[R32] 参数个数校验
来源：http://www.blog.tarul.cn/Article/details/gzzmktvrf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gvspdbxgp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fktsv.cn/Article/details/gwkmtdwfm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.tarul.cn/Article/details/gklesforr.sHtML

[R34] 退出时清理
来源：http://m.share.sjlbkw.cn/Article/details/gkwmptkzp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gbgiinkzi.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/gbimcyqfj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gznrnenwm.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gociegwcy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fktsv.cn/Article/details/gukmlqdmg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gittjmblo.sHtML

files=$(ls -1)
来源：http://3g.tarul.cn/Article/details/gxsmdvgjw.sHtML

[R38] 管道串联
来源：http://baike.epnwcf.com/Article/details/guvtuvfgy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/grppwbjbv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.yfazqb.com/Article/details/gljsfjdod.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gjmnhtpcg.sHtML

[R40] 追加写日志
来源：http://read.share.epnwcf.com/Article/details/gcbfvpoku.sHtML

echo "log" >> out.log
来源：http://read.share.sjlbkw.cn/Article/details/gbwtgcegg.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/gbumahbfo.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/gvhkroiri.sHtML

[R42] 输入重定向
来源：http://read.share.tarul.cn/Article/details/gspyitync.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/gacohgdpw.sHtML

[R43] 按名字查找文件
来源：http://www.blog.sjlbkw.cn/Article/details/gxezouqeq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.vehdjk.com/Article/details/gmpriadqh.sHtML

[R44] 按修改时间查找
来源：http://wap.fktsv.cn/Article/details/gexxtqikk.sHtML

find . -mtime -7 -type f
来源：http://read.share.fktsv.cn/Article/details/gyzlnskoc.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gbksdiwmj.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.bbcook.cn/Article/details/gjxgyqqtw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.vehdjk.com/Article/details/gvchtyecp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.epnwcf.com/Article/details/ghsksmezr.sHtML

[R47] sed 单行替换
来源：http://www.share.sjlbkw.cn/Article/details/godwpxktk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/guxaemvza.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/gipbnqkko.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/gnjgtotlo.sHtML

[R49] awk 带条件
来源：http://www.share.fktsv.cn/Article/details/ghlgblikq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.tarul.cn/Article/details/gautweacc.sHtML

[R50] awk 求和
来源：http://www.blog.epnwcf.com/Article/details/geinjnqty.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.yfazqb.com/Article/details/gfuqzxwwn.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/gtfzdpznb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.sjlbkw.cn/Article/details/gggxqhihc.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/gcxxxbzib.sHtML

wc -l a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsovhwov.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/gouqyhhak.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.sjlbkw.cn/Article/details/gbvnjatci.sHtML

[R54] 比较两个文件
来源：http://www.m.share.yfazqb.com/Article/details/gpsmoxtts.sHtML

diff a.txt b.txt
来源：http://baike.bbcook.cn/Article/details/gbdhtyzjw.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/gxbyamghs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.yfazqb.com/Article/details/gtozhighi.sHtML

[R56] 远程拷贝
来源：http://mobile.tarul.cn/Article/details/gpdioozry.sHtML

scp file user@host:/path/
来源：http://www.blog.sjlbkw.cn/Article/details/gphfkdvcq.sHtML

[R57] 远程执行命令
来源：http://wap.sjlbkw.cn/Article/details/gwozipbju.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/glkbymnnm.sHtML

[R58] 下载文件
来源：http://baike.tarul.cn/Article/details/gpxlqkgjo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.bbcook.cn/Article/details/giquqkcdy.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gokbpbwfe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.sjlbkw.cn/Article/details/gylkvmiiu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gdxnyabha.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.yfazqb.com/Article/details/gylkreygt.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/gveczetll.sHtML

df -h;  du -sh *
来源：http://3g.epnwcf.com/Article/details/gcvjixxlz.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gnlzfkaaw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/gdtmchijy.sHtML

[R63] 内存与进程
来源：http://m.share.epnwcf.com/Article/details/ghzvlwggn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.epnwcf.com/Article/details/gywyxncoz.sHtML

[R64] 结束进程
来源：http://www.share.bbcook.cn/Article/details/gxoeahoal.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/gkgyszafl.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/gcvwtmiuy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.yfazqb.com/Article/details/gvtrqrbwa.sHtML

[R66] 定时任务
来源：http://baike.tarul.cn/Article/details/gguzybbfc.sHtML

crontab -e;  crontab -l
来源：http://blog.fktsv.cn/Article/details/giyademxz.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gbiixoxhx.sHtML

openssl rand -hex 16
来源：http://wap.vehdjk.com/Article/details/gyjrhjyyb.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/gvagwebxh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/glplzwmvr.sHtML

[R69] 生成随机密码
来源：http://blog.yfazqb.com/Article/details/gflhocysy.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.sjlbkw.cn/Article/details/gzcvdtnmk.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gapkprynn.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/gepxeepau.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/grsxabspf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gpnbqxzsb.sHtML

[R72] 等待端口就绪
来源：http://3g.yfazqb.com/Article/details/gmcucmjsv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gnebcfunn.sHtML

[R73] 分割大日志
来源：http://mobile.vehdjk.com/Article/details/glmzmxpop.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/gnnzynmvt.sHtML

[R74] 批量重命名
来源：http://3g.sjlbkw.cn/Article/details/gvpcmtnfl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fktsv.cn/Article/details/gqxsrzyih.sHtML

[R75] 导出环境变量
来源：http://baike.tarul.cn/Article/details/goulcfout.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gldkshzik.sHtML

[R76] 使用临时文件
来源：http://m.share.fktsv.cn/Article/details/gdmpydvde.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gvdejylue.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/gdjgbyyqy.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/gcjvfwtzq.sHtML

[R78] 交互式菜单
来源：http://m.share.epnwcf.com/Article/details/gykopemam.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.yfazqb.com/Article/details/gaoaufhck.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gppijzwie.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gljewcwgt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gldewcwkn.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/ghupuvkit.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/goztmhxnv.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gerullils.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmdxqhjht.sHtML

[S01] C：Hello World
来源：http://www.blog.tarul.cn/Article/details/gzdfnfsfy.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/gbymugket.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.epnwcf.com/Article/details/gfdzfdkbn.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gllmrvhod.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gbzgclnzh.sHtML

[S03] C：读入整数
来源：http://m.share.fktsv.cn/Article/details/grdubajpc.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/goplaxaqh.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/grfsefvmz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gdbbxwfnt.sHtML

[S05] C：字符串长度
来源：http://read.share.vehdjk.com/Article/details/ggcbxbyzp.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/godlbvteq.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gjptidzsm.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gfyhvynzg.sHtML

[S07] C：数组遍历求和
来源：http://read.share.vehdjk.com/Article/details/gikozrmvc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.bbcook.cn/Article/details/ggchfxtab.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/gactitpug.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/goqqkiaup.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.bbcook.cn/Article/details/gntduodid.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.yfazqb.com/Article/details/gprmvtryb.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/gdkelyori.sHtML

int *p = &a;  *p = 5;
来源：http://3g.epnwcf.com/Article/details/ggcfuuara.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gowgbyttp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gdedcvwci.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gbmysubln.sHtML

fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gectltcpu.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/gpmpgorth.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/gzhqyphbx.sHtML

[S13] C：宏定义
来源：http://www.share.bbcook.cn/Article/details/goupouzyh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gtblshxhj.sHtML

[S14] C：枚举
来源：http://blog.vehdjk.com/Article/details/guxnzatff.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gtfrulmps.sHtML

[S15] C：类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gnkyirggg.sHtML

(double) a / b
来源：http://read.share.bbcook.cn/Article/details/gvqxpjoam.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/gmwllajik.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/gbaduhnou.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gawwflbbw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/gusoqaucd.sHtML

[S18] C：命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gzedwcvqf.sHtML

int main(int argc, char **argv)
来源：http://blog.fktsv.cn/Article/details/gesojgtiu.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/gehqqutpf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/garwqrwgu.sHtML

[S20] C：二分查找
来源：http://blog.sjlbkw.cn/Article/details/glfpfeanm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gekkgtgww.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/gasypxxmw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fktsv.cn/Article/details/gzbqubxad.sHtML

[S22] C：字符串转数字
来源：http://blog.vehdjk.com/Article/details/gxmibausd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.yfazqb.com/Article/details/gwnfhoeei.sHtML

[S23] C：随机数
来源：http://www.blog.sjlbkw.cn/Article/details/gahpsgwmn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/gdsiabawv.sHtML

[S24] C：获取本地时间
来源：http://mobile.vehdjk.com/Article/details/govyagokp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/gdaryxuvd.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/guvggvxtx.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/gvetujtph.sHtML

[S26] C：内存清零
来源：http://www.blog.sjlbkw.cn/Article/details/gasdpithw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.sjlbkw.cn/Article/details/gvsganhem.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/grdcibafx.sHtML

const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gbiicrhhv.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/gaittpwov.sHtML

static int counter = 0;
来源：http://baike.vehdjk.com/Article/details/geppeqcoc.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/ggnpvdtin.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gkemmdfkl.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gpcdmtasc.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gurohwkqc.sHtML

#define X_H
来源：http://www.share.vehdjk.com/Article/details/gpmtdneqw.sHtML

#endif
来源：http://www.m.share.tarul.cn/Article/details/gbtjthgfy.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gpjtnaudy.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gmlsfipei.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.bbcook.cn/Article/details/gpyodaiqw.sHtML

[S32] C++：字符串
来源：http://www.m.share.fktsv.cn/Article/details/ggxfwunqa.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gkieyiqvu.sHtML

[S33] C++：vector 增删
来源：http://www.share.fktsv.cn/Article/details/gkqdujjmz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/godewwbvf.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gahjxeznj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/gunvqpsdd.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gkitjaqzm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gcwbwrpuo.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gctmtmztg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gfcylsugr.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/gkfnloalx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gsgulnjfg.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/galgntsfb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.vehdjk.com/Article/details/goygxulkq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gqyjlgnsh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gwewadafs.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gosmerreb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/gckouhnbm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/gfkohobmd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.bbcook.cn/Article/details/gkhwqobsk.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.vehdjk.com/Article/details/gcnqugrqq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gmlacwwbb.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/glfypztkd.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.yfazqb.com/Article/details/guibekqoy.sHtML

[S44] C++：引用传参
来源：http://wap.fktsv.cn/Article/details/govhtrpxe.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gehvqiyyl.sHtML


<!-- 参考信息 -->