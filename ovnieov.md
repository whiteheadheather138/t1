代发 wailian999

[Q78] 当前时间
来源：http://3g.epnwcf.com/Article/details/grpedvido.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/gqzjiqzyd.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/gpkfnbaap.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.yfazqb.com/Article/details/gznbdbtyb.sHtML

[Q80] 字符串截取
来源：http://www.share.sjlbkw.cn/Article/details/gyooecgae.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/gydnqfpvv.sHtML

[Q81] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gestlbyyi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/gceexnnes.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fktsv.cn/Article/details/gvylssavh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gzuusbles.sHtML

[Q83] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gsukkjhwd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gjlixbgmt.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/gbjxhjacl.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/gnfynttck.sHtML

[Q85] 数值取整
来源：http://read.share.yfazqb.com/Article/details/gptqcffzi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/grgaccndw.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/glpiqjqwa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/gulsdcqry.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/gasliqiqf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fktsv.cn/Article/details/gbsbtppmb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.vehdjk.com/Article/details/gimyjjvxe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.yfazqb.com/Article/details/gtkfvnljs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.yfazqb.com/Article/details/gkwnysfll.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gljnnzjwm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/gwroqejxj.sHtML

[Q90] 生成序号列
来源：http://baike.tarul.cn/Article/details/gtylcwakl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.tarul.cn/Article/details/ghylhtowh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gminwvsos.sHtML

R. Bash 专题
来源：http://read.share.bbcook.cn/Article/details/gakazguzq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdklhmkkp.sHtML

[R01] shebang 与严格模式
来源：http://3g.fktsv.cn/Article/details/gzhkkvval.sHtML

#!/usr/bin/env bash
来源：http://blog.yfazqb.com/Article/details/grtfsatke.sHtML

set -euo pipefail
来源：http://blog.yfazqb.com/Article/details/gqsosuarm.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/gnecdjetn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.epnwcf.com/Article/details/gfblglvvu.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gdaqjmzme.sHtML

readonly PI=3.14
来源：http://blog.tarul.cn/Article/details/gcmellnlx.sHtML

[R04] 位置参数
来源：http://mobile.yfazqb.com/Article/details/gajzerwue.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gopsbhlon.sHtML

[R05] 参数默认值
来源：http://www.share.epnwcf.com/Article/details/gloqqmvvw.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/ghbgpxixm.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/gsicbplwq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gxpayyovl.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gwipllhwq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/ghmakmnyo.sHtML

[R08] 数值比较
来源：http://m.share.fktsv.cn/Article/details/gtyqqzwwu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.epnwcf.com/Article/details/gtheupddi.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gtmyfbpjs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/gguyqvlxx.sHtML

[R10] 正则匹配
来源：http://baike.bbcook.cn/Article/details/gpcnzthbz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gcsrxdqpd.sHtML

[R11] case 多分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuvqqoaw.sHtML

case "$1" in
来源：http://wap.yfazqb.com/Article/details/gjpyoqmik.sHtML

start) echo "启动" ;;
来源：http://read.share.yfazqb.com/Article/details/gqtstgikd.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.epnwcf.com/Article/details/gkjcruvmj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fktsv.cn/Article/details/gjhqiweuf.sHtML

esac
来源：http://m.share.tarul.cn/Article/details/gaggfpcdy.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/glljfhwpg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/gkzdhjmuq.sHtML

[R13] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gjjjawiyb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gyjxqwiwc.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/gzvfewrso.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/givwuokun.sHtML

[R15] while 逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gvapajwqc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gtewvzetw.sHtML

[R16] until 等待条件
来源：http://3g.fktsv.cn/Article/details/gxiwlwdcr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gdswtedwa.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfphhkex.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gqqoujaur.sHtML

[R18] 遍历数组
来源：http://blog.sjlbkw.cn/Article/details/ggzwaseyw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/ggriomtjk.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/guqrfepyg.sHtML

echo "${#arr[@]}"
来源：http://mobile.vehdjk.com/Article/details/gtmrygvtx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/gmjrmajnp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gygupnfjn.sHtML

[R21] 字符串长度
来源：http://baike.vehdjk.com/Article/details/gdqpyevtg.sHtML

echo "${#s}"
来源：http://www.m.share.bbcook.cn/Article/details/gwcmohtsg.sHtML

[R22] 截取子串
来源：http://baike.yfazqb.com/Article/details/gbyxxqwqc.sHtML

echo "${s:0:5}"
来源：http://wap.tarul.cn/Article/details/gevsajhnx.sHtML

[R23] 字符串替换
来源：http://www.m.share.vehdjk.com/Article/details/gkemsgnnu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.yfazqb.com/Article/details/gqkfyqase.sHtML

[R24] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gvhryfkcu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.bbcook.cn/Article/details/garewgzlb.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.bbcook.cn/Article/details/gtfxhdcva.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.yfazqb.com/Article/details/gxjakhyio.sHtML

[R26] 命令替换
来源：http://blog.sjlbkw.cn/Article/details/gwbvirokb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/gpnxaannk.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/gzyhxkcfd.sHtML

echo $((1 + 2 * 3))
来源：http://wap.yfazqb.com/Article/details/gcxuqixmh.sHtML

[R28] 浮点运算
来源：http://wap.epnwcf.com/Article/details/gqsnbtzfq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fktsv.cn/Article/details/gmmlcejth.sHtML

[R29] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gvbcqzcxo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/gzeaojwqk.sHtML

[R30] 函数返回状态码
来源：http://mobile.fktsv.cn/Article/details/gadaxserq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/gogujmzcj.sHtML

[R31] 局部变量
来源：http://blog.fktsv.cn/Article/details/ganoremqg.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fktsv.cn/Article/details/gadjtgglk.sHtML

[R32] 参数个数校验
来源：http://www.m.share.vehdjk.com/Article/details/gfujzfsgl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gotzqzybe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.vehdjk.com/Article/details/gcyinoreb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.bbcook.cn/Article/details/gdzptoymw.sHtML

[R34] 退出时清理
来源：http://baike.vehdjk.com/Article/details/gtmbpprpf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/gexkkxugw.sHtML

[R35] 后台执行并等待
来源：http://read.share.fktsv.cn/Article/details/gdcgevgbw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gerifdxsw.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gkqeqoqhc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fktsv.cn/Article/details/gsavpzkat.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/gbitcqfnj.sHtML

files=$(ls -1)
来源：http://www.m.share.vehdjk.com/Article/details/gxtanzdku.sHtML

[R38] 管道串联
来源：http://www.blog.sjlbkw.cn/Article/details/gpfbeyxvj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/glbefthfe.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.sjlbkw.cn/Article/details/gahxdezxf.sHtML

cmd > out.log 2>&1
来源：http://mobile.yfazqb.com/Article/details/gfbwpcpvj.sHtML

[R40] 追加写日志
来源：http://mobile.epnwcf.com/Article/details/grvchaloi.sHtML

echo "log" >> out.log
来源：http://baike.vehdjk.com/Article/details/ggpcatyhc.sHtML

[R41] 丢弃输出
来源：http://baike.fktsv.cn/Article/details/gfouyphso.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gghaxpaan.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/grviqfnco.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/gqqftwsjh.sHtML

[R43] 按名字查找文件
来源：http://3g.sjlbkw.cn/Article/details/giijjllqm.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fktsv.cn/Article/details/gwoftckua.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gxytodqwj.sHtML

find . -mtime -7 -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gexyrluol.sHtML

[R45] 批量删除
来源：http://blog.epnwcf.com/Article/details/gjaxsarrd.sHtML

find . -name "*.tmp" -delete
来源：http://wap.tarul.cn/Article/details/gihwsavpb.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/gkbwpdogo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.tarul.cn/Article/details/gvoispcxf.sHtML

[R47] sed 单行替换
来源：http://baike.yfazqb.com/Article/details/gdrwarqrk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.yfazqb.com/Article/details/gjaheqvuy.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/gxgkozqov.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gxuewbphu.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/gbubamdpo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/gqvhxjblx.sHtML

[R50] awk 求和
来源：http://www.blog.sjlbkw.cn/Article/details/gtfvbmdzp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gcmnggwih.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fktsv.cn/Article/details/geueekikm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.epnwcf.com/Article/details/gdkfkzzwo.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/glugpgcyz.sHtML

wc -l a.txt
来源：http://m.share.yfazqb.com/Article/details/gdbowxipu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fktsv.cn/Article/details/gcuetogbk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.tarul.cn/Article/details/glnnugtfh.sHtML

[R54] 比较两个文件
来源：http://read.share.yfazqb.com/Article/details/gwheqcxyg.sHtML

diff a.txt b.txt
来源：http://mobile.fktsv.cn/Article/details/gghnhpkxx.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/gearacvwh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.tarul.cn/Article/details/gwzlvozar.sHtML

[R56] 远程拷贝
来源：http://baike.fktsv.cn/Article/details/gmkcemfpp.sHtML

scp file user@host:/path/
来源：http://m.share.epnwcf.com/Article/details/gmonjvluj.sHtML

[R57] 远程执行命令
来源：http://read.share.tarul.cn/Article/details/gwihwlsvf.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/gafmjdwme.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gtvjouvzn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.vehdjk.com/Article/details/ghndhzjkl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gmcvnbjsu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/gyhluhvwj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gapzcjmde.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/garjpzula.sHtML

[R61] 磁盘占用
来源：http://read.share.fktsv.cn/Article/details/gbgzfqjah.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/gqszojmpd.sHtML

[R62] 找最占空间的文件
来源：http://baike.epnwcf.com/Article/details/gdyapalge.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/gcbtnmpga.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/glufchnhq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpasbijt.sHtML

[R64] 结束进程
来源：http://m.share.tarul.cn/Article/details/gqyenzskl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.tarul.cn/Article/details/ghaorofqc.sHtML

[R65] 查看端口占用
来源：http://blog.fktsv.cn/Article/details/gavzupwme.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.bbcook.cn/Article/details/gtqytlzat.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gnzjeqlwf.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.epnwcf.com/Article/details/gtgwszvsl.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxuueajl.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gkqavtiem.sHtML

[R68] 计算文件校验值
来源：http://m.share.bbcook.cn/Article/details/gplhzpzbl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.yfazqb.com/Article/details/gudtgustb.sHtML

[R69] 生成随机密码
来源：http://3g.vehdjk.com/Article/details/gcdxjieoh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.bbcook.cn/Article/details/gbktqldbg.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/gvgizzlqy.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/gvgmxymxs.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/geagdnpia.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gtbzzwwkk.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/gzitoevdy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/ggmhwnfbe.sHtML

[R73] 分割大日志
来源：http://read.share.vehdjk.com/Article/details/gzgapgfhq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gwwqfadys.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/groaxxokr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.vehdjk.com/Article/details/gbsecjcso.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gqncggyzc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.vehdjk.com/Article/details/gtztfkcrw.sHtML

[R76] 使用临时文件
来源：http://baike.fktsv.cn/Article/details/gtqpibswc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gcgrxyhtg.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/gwovlerea.sHtML

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gojcxltob.sHtML

[R78] 交互式菜单
来源：http://www.share.yfazqb.com/Article/details/glzyhhhgx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/grwkyydtz.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/gtnyoltuu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/glcyguhwh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.tarul.cn/Article/details/gjsktnewt.sHtML

time ./run.sh
来源：http://3g.yfazqb.com/Article/details/gvpjnztij.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmdapghcx.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/gvxpsiimk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbtdltedf.sHtML

[S01] C：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gnvgdlirl.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/geufimzru.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/giofomgfw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.bbcook.cn/Article/details/gggszzbej.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.yfazqb.com/Article/details/gnhrwvywb.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gifpawpki.sHtML

int x; scanf("%d", &x);
来源：http://baike.sjlbkw.cn/Article/details/grpimwhum.sHtML

[S04] C：字符串复制
来源：http://read.share.tarul.cn/Article/details/glhyvfurx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.vehdjk.com/Article/details/gcluucdbn.sHtML

[S05] C：字符串长度
来源：http://mobile.vehdjk.com/Article/details/gnhkjnmsb.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/ggwufbigq.sHtML

[S06] C：字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gcgpubfkv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/gfdiosssu.sHtML

[S07] C：数组遍历求和
来源：http://read.share.yfazqb.com/Article/details/gtdllcryw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/gjboxxtib.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gytyqjuii.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.sjlbkw.cn/Article/details/gfgoxkjco.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gbyyhtsqj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/grsxlzcha.sHtML

[S10] C：指针与解引用
来源：http://m.share.tarul.cn/Article/details/gueceeyoq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/gqvpxezkv.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/giuwjtoyt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.tarul.cn/Article/details/ggtdqvzze.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.sjlbkw.cn/Article/details/gepggguit.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/geaovfkkp.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/ggymvljol.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gghrdhrtf.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gvzwicruy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fktsv.cn/Article/details/gvrounizh.sHtML

[S14] C：枚举
来源：http://blog.yfazqb.com/Article/details/geygfnmxo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.tarul.cn/Article/details/gxliasnec.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gzohhnrbk.sHtML

(double) a / b
来源：http://www.m.share.bbcook.cn/Article/details/gyrfrrzkb.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/gdwrzppkl.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/gjxrfgesu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fktsv.cn/Article/details/gymxcsrkf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fktsv.cn/Article/details/gthbxpeiz.sHtML

[S18] C：命令行参数
来源：http://blog.epnwcf.com/Article/details/gyzxhypit.sHtML

int main(int argc, char **argv)
来源：http://mobile.tarul.cn/Article/details/gzjvilnkm.sHtML

[S19] C：快速排序
来源：http://3g.vehdjk.com/Article/details/gyvrdnyie.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gnznxoanj.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/gycrjfiyy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gyzbtfanr.sHtML

[S21] C：字符类别判断
来源：http://blog.epnwcf.com/Article/details/gxpikrqsg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gecvdmxlj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gmpbipzzo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.tarul.cn/Article/details/gqezwmqnk.sHtML

[S23] C：随机数
来源：http://read.share.yfazqb.com/Article/details/gcdzwhxge.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.epnwcf.com/Article/details/gboiokgmv.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gqfugwqmn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/giahvanlc.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gvrozlklz.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/goxucceuk.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gkpjbhhxs.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.tarul.cn/Article/details/gcsizijbd.sHtML

[S27] C：定义常量
来源：http://baike.fktsv.cn/Article/details/gvecpszau.sHtML

const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gkiubpoml.sHtML

[S28] C：静态变量
来源：http://www.m.share.fktsv.cn/Article/details/gnthsbpyp.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gdnzkoedb.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/gzrjddbdn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/gvlkebxfo.sHtML

[S30] C：头文件保护
来源：http://mobile.sjlbkw.cn/Article/details/gtdxyaflr.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/ggkvjaxki.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/grivqxhnx.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/ghoskogmw.sHtML

[S31] C++：Hello World
来源：http://mobile.yfazqb.com/Article/details/gfhkgevoc.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/guxflbzjv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/gystjksqq.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/grmtudwuz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gpgmtzdro.sHtML

[S33] C++：vector 增删
来源：http://baike.fktsv.cn/Article/details/gfrgsvlcv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gbmxoaaqo.sHtML

[S34] C++：遍历 vector
来源：http://m.share.yfazqb.com/Article/details/gpatpkror.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.tarul.cn/Article/details/grihvwvdk.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/gmjvsxohc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gybnvefne.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gpsqwcesw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gzmqrmoda.sHtML

[S37] C++：set
来源：http://www.share.tarul.cn/Article/details/gcrcrexzi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gmuyflpfo.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/gbbclvold.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/gcvodawwk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.bbcook.cn/Article/details/grvvhxlaf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/gufoatrrl.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/ghooxmfqm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.bbcook.cn/Article/details/gdyyisuzx.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/ghxdrqdxb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.vehdjk.com/Article/details/glowyhrkx.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.tarul.cn/Article/details/gglgibirm.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gvelixzdx.sHtML

[S43] C++：智能指针
来源：http://wap.sjlbkw.cn/Article/details/gzhlcvlnp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.bbcook.cn/Article/details/giauufprt.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/gnecvedjt.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.epnwcf.com/Article/details/gxklfgobm.sHtML

[S45] C++：lambda
来源：http://3g.vehdjk.com/Article/details/gokerpdjj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gsrdqrous.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gztnnhxvc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fktsv.cn/Article/details/gafdhnirb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/gxqecewsn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/gmbvobfim.sHtML

[S48] C++：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gxvchsqxt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/gzlhdhfxb.sHtML


<!-- 参考信息 -->