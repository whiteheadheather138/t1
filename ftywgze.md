代发 wailian999

[Q76] 按天统计
来源：http://read.share.tarul.cn/Article/details/gjyhqossd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fktsv.cn/Article/details/gaczgdunu.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/gfepkzedy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.bbcook.cn/Article/details/grtngpauw.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/gcbvwrewb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.epnwcf.com/Article/details/gyqpwajlu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gwqfyryko.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.tarul.cn/Article/details/gbmfulzbz.sHtML

[Q80] 字符串截取
来源：http://wap.vehdjk.com/Article/details/gdgirocub.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/ggbydcxir.sHtML

[Q81] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gnqbjqtsy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.vehdjk.com/Article/details/gemmprieu.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.vehdjk.com/Article/details/gnbzvavcw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gnihqbdlg.sHtML

[Q83] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gleqoeyud.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gsvlkxsll.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/grarlhyms.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gdxczqpow.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gjyoebmwz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/gwpcoyulh.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.sjlbkw.cn/Article/details/gftlfvqce.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fktsv.cn/Article/details/gvkynlwxz.sHtML

[Q87] JSON 字段做条件
来源：http://wap.vehdjk.com/Article/details/gyrtcrfmb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnbsdbkn.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.sjlbkw.cn/Article/details/gvdfpqpvk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/gncxfnjeh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.yfazqb.com/Article/details/gawqpwjtb.sHtML

[Q89] 判断表是否存在
来源：http://baike.tarul.cn/Article/details/gnwlfdhsu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/gcontmioh.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/gwupbzxli.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.yfazqb.com/Article/details/gvydbsqqs.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfxgjidpj.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/glqjdwjoe.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggzkowyfc.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.vehdjk.com/Article/details/gmuevawpz.sHtML

#!/usr/bin/env bash
来源：http://baike.bbcook.cn/Article/details/gkdwtagmi.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/gtnbanvpx.sHtML

[R02] 变量赋值与使用
来源：http://3g.tarul.cn/Article/details/gdzncpxbs.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/gytxbunth.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/gptajuxjz.sHtML

readonly PI=3.14
来源：http://www.m.share.bbcook.cn/Article/details/gqwzhaftd.sHtML

[R04] 位置参数
来源：http://read.share.tarul.cn/Article/details/golfwdoqn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gggneuhwf.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/gxhnuwwyz.sHtML

name="${1:-default}"
来源：http://www.blog.fktsv.cn/Article/details/ghjejsgqn.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/gtukaccrp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gmhyzypdg.sHtML

[R07] if 判断文件
来源：http://blog.tarul.cn/Article/details/gcfxppkgh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.tarul.cn/Article/details/ggekayova.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gmyvfmadd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/gwdqydjqi.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gnyvcnayx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.tarul.cn/Article/details/gebbejpcn.sHtML

[R10] 正则匹配
来源：http://3g.tarul.cn/Article/details/gdgwmqhpc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.epnwcf.com/Article/details/ghgfvoifu.sHtML

[R11] case 多分支
来源：http://blog.fktsv.cn/Article/details/gvtfohwug.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/gubkiqdvm.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gpphzflmq.sHtML

stop)  echo "停止" ;;
来源：http://blog.yfazqb.com/Article/details/gmarutrwa.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/gmbubikoj.sHtML

esac
来源：http://read.share.vehdjk.com/Article/details/gxkwmxppf.sHtML

[R12] for 遍历文件
来源：http://mobile.yfazqb.com/Article/details/gkcjrnuxm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/gjfvuoldq.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gdyupqxhz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gudxxkeef.sHtML

[R14] C 风格 for
来源：http://read.share.epnwcf.com/Article/details/gzwjmlbxm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gjfvtifhy.sHtML

[R15] while 逐行读文件
来源：http://blog.vehdjk.com/Article/details/gcoekvzrk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gnymvhojh.sHtML

[R16] until 等待条件
来源：http://www.m.share.fktsv.cn/Article/details/guqszbphk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gxppaqddx.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/gbcayqdiy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gpohyxobm.sHtML

[R18] 遍历数组
来源：http://baike.sjlbkw.cn/Article/details/gehrlikdy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/gggwwqgho.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gfyugmrql.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gpshgrxhe.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/gbldmnaea.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.bbcook.cn/Article/details/guibruptl.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/grjwlauoi.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gjjcvxuzu.sHtML

[R22] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gifvujpgh.sHtML

echo "${s:0:5}"
来源：http://www.m.share.tarul.cn/Article/details/gyzasqciw.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gdphlcaib.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/ghksoiehb.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/glbyhfnbz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fktsv.cn/Article/details/gpojpiqjg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gohwpkytp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/gujrxrlov.sHtML

[R26] 命令替换
来源：http://read.share.tarul.cn/Article/details/gqhkrnbxu.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gbdseqsiz.sHtML

[R27] 算术展开
来源：http://read.share.fktsv.cn/Article/details/gheudyxtj.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.epnwcf.com/Article/details/grwudkiln.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gpzjplfbi.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.bbcook.cn/Article/details/gcojabarj.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/glfbtuvcw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.bbcook.cn/Article/details/gbsabhzgh.sHtML

[R30] 函数返回状态码
来源：http://www.share.sjlbkw.cn/Article/details/ggkdfzjpg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.tarul.cn/Article/details/gawhfwqdh.sHtML

[R31] 局部变量
来源：http://www.m.share.vehdjk.com/Article/details/ghsitdmbm.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/gxjafniqf.sHtML

[R32] 参数个数校验
来源：http://baike.yfazqb.com/Article/details/glmsqmchd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gwajoakdy.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/gqvjnyoew.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.epnwcf.com/Article/details/gncsrsxhx.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/gfqxxfyru.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/gsfjfdzgp.sHtML

[R35] 后台执行并等待
来源：http://www.share.vehdjk.com/Article/details/gxrlbakpa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fktsv.cn/Article/details/gtrntmcwu.sHtML

[R36] 并发执行多个任务
来源：http://baike.epnwcf.com/Article/details/gxxnqrezd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/ghmwgweil.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.vehdjk.com/Article/details/gqqholond.sHtML

files=$(ls -1)
来源：http://blog.epnwcf.com/Article/details/gngztdbvi.sHtML

[R38] 管道串联
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyuxvkum.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gjelytkrb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.epnwcf.com/Article/details/gcgupveoz.sHtML

cmd > out.log 2>&1
来源：http://mobile.epnwcf.com/Article/details/gcczontle.sHtML

[R40] 追加写日志
来源：http://read.share.bbcook.cn/Article/details/gjooxixio.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/gciuoffoq.sHtML

[R41] 丢弃输出
来源：http://wap.yfazqb.com/Article/details/gisfobteb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gbpqyvjiq.sHtML

[R42] 输入重定向
来源：http://baike.bbcook.cn/Article/details/gszeacgdz.sHtML

wc -l < a.txt
来源：http://read.share.tarul.cn/Article/details/gmebpxjiz.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/gdestovao.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fktsv.cn/Article/details/gceaooani.sHtML

[R44] 按修改时间查找
来源：http://m.share.yfazqb.com/Article/details/gkejhcmxl.sHtML

find . -mtime -7 -type f
来源：http://read.share.vehdjk.com/Article/details/gnuibijab.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/gclliylvb.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.epnwcf.com/Article/details/gfoaagtfr.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.vehdjk.com/Article/details/gitbqoawc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.tarul.cn/Article/details/glxyppkoo.sHtML

[R47] sed 单行替换
来源：http://wap.epnwcf.com/Article/details/gqkwisqys.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gddsuraaz.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/gvrewlcwj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.epnwcf.com/Article/details/gyyqadecx.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/ghqcowodi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.sjlbkw.cn/Article/details/gblqzwycu.sHtML

[R50] awk 求和
来源：http://wap.epnwcf.com/Article/details/glbogmggm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gzfkwazop.sHtML

[R51] 排序去重取前几
来源：http://blog.tarul.cn/Article/details/gyfkicozf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gqdhqjbfc.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gsjuotryu.sHtML

wc -l a.txt
来源：http://blog.vehdjk.com/Article/details/gutbwrutj.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.yfazqb.com/Article/details/gicohptux.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/gtohcnkwo.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/gpfkxshok.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/gnfsoithp.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gejieywxi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.bbcook.cn/Article/details/goceybtgl.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gfeffomqi.sHtML

scp file user@host:/path/
来源：http://wap.sjlbkw.cn/Article/details/glpmcffmz.sHtML

[R57] 远程执行命令
来源：http://read.share.fktsv.cn/Article/details/ggbgiurdd.sHtML

ssh user@host 'uptime'
来源：http://3g.yfazqb.com/Article/details/gmykywcru.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gndrvhsjj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/geoplyafk.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gqcjbyqbe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.sjlbkw.cn/Article/details/gdpqgyqgl.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/ggfzunvkq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.tarul.cn/Article/details/gnluquwew.sHtML

[R61] 磁盘占用
来源：http://www.m.share.vehdjk.com/Article/details/gtnjzeatf.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/gydzfklcd.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/guspatoaz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.tarul.cn/Article/details/ghtxjaacr.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/grzjvaaks.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/gjrcznuza.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/gdetodukh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.bbcook.cn/Article/details/gnmczysjb.sHtML

[R65] 查看端口占用
来源：http://blog.epnwcf.com/Article/details/gyrqdgntt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.sjlbkw.cn/Article/details/gofnaqslu.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/gzxeizxcb.sHtML

crontab -e;  crontab -l
来源：http://mobile.fktsv.cn/Article/details/gygwbyill.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.tarul.cn/Article/details/gzopwpykg.sHtML

openssl rand -hex 16
来源：http://www.m.share.sjlbkw.cn/Article/details/gurbymynt.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.yfazqb.com/Article/details/gjkodrlyb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/gvbfgjnwd.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/gnsnungco.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/gvuwuljkm.sHtML

[R70] 时间戳与互转
来源：http://blog.fktsv.cn/Article/details/gtahxuqnm.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/gbxxwzwss.sHtML

[R71] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gyeqoeisv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gsnqqposz.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/gwfpliyco.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gnhdiqnxz.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/grvhzllxp.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/gzyatrqra.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/gpjqoaedx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.bbcook.cn/Article/details/gdtacmyky.sHtML

[R75] 导出环境变量
来源：http://m.share.fktsv.cn/Article/details/gtcmhqwmj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/gjhtjxfqf.sHtML

[R76] 使用临时文件
来源：http://3g.yfazqb.com/Article/details/gzkqevimv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gihnyllvq.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gcfqijjfy.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/guzhuezsr.sHtML

[R78] 交互式菜单
来源：http://www.share.sjlbkw.cn/Article/details/gnmuyvneh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.tarul.cn/Article/details/goiisyibb.sHtML

[R79] 解析命令行选项
来源：http://www.share.tarul.cn/Article/details/gxuoucnfl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gujniopjq.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/geqbcqeja.sHtML

time ./run.sh
来源：http://wap.bbcook.cn/Article/details/gdbzbumgg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gghjoskbe.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/ghfsseffy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gskguqqrq.sHtML

[S01] C：Hello World
来源：http://mobile.fktsv.cn/Article/details/gbcfyhdit.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/gwhicpxyw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.epnwcf.com/Article/details/gldlwpvnw.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/ggbnvzjva.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.vehdjk.com/Article/details/gbaqlxzat.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gghzmqkgx.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gauyaqwom.sHtML

[S04] C：字符串复制
来源：http://m.share.sjlbkw.cn/Article/details/gqkyvvgll.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/gtcgjoubx.sHtML

[S05] C：字符串长度
来源：http://www.share.vehdjk.com/Article/details/gobgfdjmq.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gtyyccwks.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gqkvnmctm.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fktsv.cn/Article/details/gmavlbimh.sHtML

[S07] C：数组遍历求和
来源：http://m.share.sjlbkw.cn/Article/details/gugotbefu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.sjlbkw.cn/Article/details/gdktfadmr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.tarul.cn/Article/details/gqqvadler.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/gyeydjovn.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/godbyqhdz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gwinmnzix.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/gudbasrfu.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gabpttdxk.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gaggfvhna.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/gtbjabwxj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fktsv.cn/Article/details/gmwrlwewt.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gzblvxjcb.sHtML

[S12] C：写文件
来源：http://baike.fktsv.cn/Article/details/gmvgcxofg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/ginrznees.sHtML

[S13] C：宏定义
来源：http://blog.tarul.cn/Article/details/geuupdcpd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/gflilaoil.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gvsawhinb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/gqrzjsduc.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/groeaklpf.sHtML

(double) a / b
来源：http://m.share.epnwcf.com/Article/details/gqbaevnmx.sHtML

[S16] C：位操作置位
来源：http://mobile.yfazqb.com/Article/details/gcnbyklse.sHtML

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gjuggtrwf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.vehdjk.com/Article/details/gjjuvqgne.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.vehdjk.com/Article/details/guwiqociv.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gsdbejgvu.sHtML

int main(int argc, char **argv)
来源：http://m.share.yfazqb.com/Article/details/guchbkwrl.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/ghaihelqi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/grsdxplzc.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/gjmevypqs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gwesunznx.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/gvaumpqpy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/gvqlaacdz.sHtML

[S22] C：字符串转数字
来源：http://blog.fktsv.cn/Article/details/gnwdvfmhj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/grovejhcj.sHtML

[S23] C：随机数
来源：http://blog.yfazqb.com/Article/details/gorjlirai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/gqfyjfqsd.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/gwvjlqcwk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.yfazqb.com/Article/details/glipvkxvu.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/grtbdwzsa.sHtML

memcpy(dst, src, n);
来源：http://wap.fktsv.cn/Article/details/gwmhtzhcu.sHtML

[S26] C：内存清零
来源：http://m.share.sjlbkw.cn/Article/details/ghbimkybq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gwdgooydu.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/gugrtonpz.sHtML

const double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gkctvnhng.sHtML

[S28] C：静态变量
来源：http://baike.fktsv.cn/Article/details/giqwaalgu.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/gjnnmxenj.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/gxychnqao.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/gruvnjdta.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/giaddwkwj.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/gkkexdvsf.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/glcsnpyof.sHtML

#endif
来源：http://www.share.vehdjk.com/Article/details/glfmahgcm.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gqzqpdkoe.sHtML

#include <iostream>
来源：http://www.share.tarul.cn/Article/details/gvpqlchkd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.epnwcf.com/Article/details/gdzbvgrmr.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gxvcuwoju.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fktsv.cn/Article/details/gokuhcidz.sHtML

[S33] C++：vector 增删
来源：http://read.share.tarul.cn/Article/details/gkdwxfjoa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/gnzjyvfcn.sHtML

[S34] C++：遍历 vector
来源：http://wap.sjlbkw.cn/Article/details/gvmirmken.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gfxyeipsm.sHtML

[S35] C++：map
来源：http://www.share.fktsv.cn/Article/details/gwrkxcnbs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gjlauophy.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/ghyjgmwrm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gkfqdkbfz.sHtML

[S37] C++：set
来源：http://www.share.yfazqb.com/Article/details/goznxmurr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.vehdjk.com/Article/details/ggqvrcrox.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/graheijpo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.tarul.cn/Article/details/glsusgpib.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.sjlbkw.cn/Article/details/gcrhmfwzh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gbxefhquq.sHtML

[S40] C++：查找元素
来源：http://3g.fktsv.cn/Article/details/gzeimmgxv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/guygediqz.sHtML

[S41] C++：类与构造函数
来源：http://www.share.vehdjk.com/Article/details/gofisyerb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/ggcteaqfx.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqnszfjj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/glwxmujfx.sHtML

[S43] C++：智能指针
来源：http://www.blog.tarul.cn/Article/details/givogokwr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/gvkradfjn.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/gwnfqhcqr.sHtML

void inc(int &x) { ++x; }
来源：http://blog.sjlbkw.cn/Article/details/gshawwwrn.sHtML

[S45] C++：lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gbexkmasg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fktsv.cn/Article/details/gmnkfpqoy.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/glnvcwbfl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/gdugfvrmz.sHtML


<!-- 参考信息 -->