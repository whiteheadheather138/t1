代发 wailian999

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/glxgtrtug.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.bbcook.cn/Article/details/gnnykppcw.sHtML

[Q79] 字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gjuteksgm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.vehdjk.com/Article/details/ggoywwobt.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/gdopasviy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gdstqwxqq.sHtML

[Q81] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gwzoirkkz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/godtbvgwo.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.yfazqb.com/Article/details/gndxldpks.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gxpnexybx.sHtML

[Q83] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gbxdnugbu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gcrbixmix.sHtML

[Q84] 去除首尾空格
来源：http://blog.sjlbkw.cn/Article/details/govmsqbmc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gfaxpltjn.sHtML

[Q85] 数值取整
来源：http://www.blog.yfazqb.com/Article/details/gkxyfnhsu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/glvkhfsli.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.sjlbkw.cn/Article/details/gzbqwhckj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/gmuhhfhdf.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.epnwcf.com/Article/details/gbdbxchsn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.vehdjk.com/Article/details/gvrtjqxmx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/gvuhmunwl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/gzfryeetz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/ghtchwtpd.sHtML

[Q89] 判断表是否存在
来源：http://blog.vehdjk.com/Article/details/ghhdanrsv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.tarul.cn/Article/details/gogfxcyqp.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/gphmeyugw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.epnwcf.com/Article/details/gsxfcdlod.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqxhejks.sHtML

R. Bash 专题
来源：http://www.m.share.fktsv.cn/Article/details/gvvychytk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghtgmcakr.sHtML

[R01] shebang 与严格模式
来源：http://wap.vehdjk.com/Article/details/gmdcwzowy.sHtML

#!/usr/bin/env bash
来源：http://read.share.yfazqb.com/Article/details/gmhkrffhy.sHtML

set -euo pipefail
来源：http://mobile.yfazqb.com/Article/details/gyqduhwrd.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.sjlbkw.cn/Article/details/gjkiyamwq.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/gyitcaker.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/gawsggoog.sHtML

readonly PI=3.14
来源：http://wap.tarul.cn/Article/details/gjygyqbwr.sHtML

[R04] 位置参数
来源：http://blog.sjlbkw.cn/Article/details/gqbneaxdl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/ggyyhdhjw.sHtML

[R05] 参数默认值
来源：http://wap.yfazqb.com/Article/details/gepriehzn.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/gopegdawe.sHtML

[R06] 判断命令是否存在
来源：http://baike.epnwcf.com/Article/details/gtbnahahd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gybxpuvlm.sHtML

[R07] if 判断文件
来源：http://read.share.vehdjk.com/Article/details/gjszhncky.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.sjlbkw.cn/Article/details/gpgdvngms.sHtML

[R08] 数值比较
来源：http://blog.vehdjk.com/Article/details/ghabzzdaf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fktsv.cn/Article/details/guhqtjbtm.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/grghchtyi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/gvfcbglne.sHtML

[R10] 正则匹配
来源：http://read.share.epnwcf.com/Article/details/giduznnpj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/gqwcjhaoq.sHtML

[R11] case 多分支
来源：http://www.blog.vehdjk.com/Article/details/gveeabagh.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/gkjbowbhh.sHtML

start) echo "启动" ;;
来源：http://www.blog.fktsv.cn/Article/details/guphyyyoy.sHtML

stop)  echo "停止" ;;
来源：http://wap.epnwcf.com/Article/details/gmtmublkc.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/ghpnrtoat.sHtML

esac
来源：http://blog.tarul.cn/Article/details/guuibupzs.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/gzdjmmdqx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gweeldzak.sHtML

[R13] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/ggolkvxqz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/ghywdukdd.sHtML

[R14] C 风格 for
来源：http://www.share.tarul.cn/Article/details/gssyqfbrh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gxfdkqlla.sHtML

[R15] while 逐行读文件
来源：http://wap.tarul.cn/Article/details/gpkyoofzz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/gthqkyoix.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/gmjccvsbw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gknjbamyu.sHtML

[R17] 数组定义与取值
来源：http://baike.sjlbkw.cn/Article/details/gvxvfheid.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fktsv.cn/Article/details/gnumwwaqp.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/ghuxxbuna.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.epnwcf.com/Article/details/gfrimxgqf.sHtML

[R19] 数组长度
来源：http://wap.bbcook.cn/Article/details/ghzwasjas.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/ghfxhjyyw.sHtML

[R20] 关联数组（字典）
来源：http://baike.vehdjk.com/Article/details/ghntkdslk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.epnwcf.com/Article/details/gmftupqry.sHtML

[R21] 字符串长度
来源：http://wap.fktsv.cn/Article/details/ggkrtjfti.sHtML

echo "${#s}"
来源：http://wap.yfazqb.com/Article/details/geosczzwp.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/guwdugajc.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/gadcvggud.sHtML

[R23] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gesngbyri.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/gefwkmxmr.sHtML

[R24] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gdilyvqpq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/gfcwrmtth.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.tarul.cn/Article/details/glnqlvywn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/gfzndgspk.sHtML

[R26] 命令替换
来源：http://wap.bbcook.cn/Article/details/gscvvyxud.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.vehdjk.com/Article/details/gwadmbjma.sHtML

[R27] 算术展开
来源：http://blog.fktsv.cn/Article/details/gduppjiby.sHtML

echo $((1 + 2 * 3))
来源：http://3g.tarul.cn/Article/details/geryyvtut.sHtML

[R28] 浮点运算
来源：http://baike.sjlbkw.cn/Article/details/gzfubeqif.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.tarul.cn/Article/details/gwugkpuil.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gjonbxuls.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.epnwcf.com/Article/details/gocmtjovc.sHtML

[R30] 函数返回状态码
来源：http://3g.tarul.cn/Article/details/gssyupfws.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/gifhlxldb.sHtML

[R31] 局部变量
来源：http://www.blog.epnwcf.com/Article/details/gcvftxoxy.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.yfazqb.com/Article/details/gcdrmjieo.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gkcuafiye.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gnleapkcy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/gvjhzxtdl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/gkfdrotrh.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/ghokrthjw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/glvzpqtqp.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.vehdjk.com/Article/details/ggkqvwmbn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.vehdjk.com/Article/details/gznmmlbji.sHtML

[R36] 并发执行多个任务
来源：http://baike.vehdjk.com/Article/details/gpljwdtur.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.yfazqb.com/Article/details/glfotfhsg.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gnvlvgvvm.sHtML

files=$(ls -1)
来源：http://www.m.share.vehdjk.com/Article/details/gknexfxox.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gppgozohm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.tarul.cn/Article/details/grhqidbcf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.vehdjk.com/Article/details/gkjkkhmlr.sHtML

cmd > out.log 2>&1
来源：http://baike.epnwcf.com/Article/details/gwewvsprz.sHtML

[R40] 追加写日志
来源：http://blog.sjlbkw.cn/Article/details/gowpdiieh.sHtML

echo "log" >> out.log
来源：http://www.m.share.bbcook.cn/Article/details/gjzqhwlop.sHtML

[R41] 丢弃输出
来源：http://www.share.sjlbkw.cn/Article/details/gqowwesjl.sHtML

cmd >/dev/null 2>&1
来源：http://blog.epnwcf.com/Article/details/guhwjwhak.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/gekhriatw.sHtML

wc -l < a.txt
来源：http://wap.tarul.cn/Article/details/gxezuulpc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gqouzkuxo.sHtML

find . -name "*.log" -type f
来源：http://read.share.bbcook.cn/Article/details/glefxvzrh.sHtML

[R44] 按修改时间查找
来源：http://www.blog.tarul.cn/Article/details/gkpuglkry.sHtML

find . -mtime -7 -type f
来源：http://mobile.yfazqb.com/Article/details/gitvdmryk.sHtML

[R45] 批量删除
来源：http://wap.bbcook.cn/Article/details/ggekqmxya.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/glkpczqlr.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.epnwcf.com/Article/details/glybkymym.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/gnaubapru.sHtML

[R47] sed 单行替换
来源：http://mobile.yfazqb.com/Article/details/gfvfydxfn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gmrcivhob.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/gwwskmlqz.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fktsv.cn/Article/details/gjujqheuh.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gftymevqn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/glcynmrwp.sHtML

[R50] awk 求和
来源：http://read.share.yfazqb.com/Article/details/gwfzxnukx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/gvjdluxsc.sHtML

[R51] 排序去重取前几
来源：http://wap.tarul.cn/Article/details/gweognmhm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/gczhcbddy.sHtML

[R52] 统计行数
来源：http://m.share.fktsv.cn/Article/details/giueyzyvp.sHtML

wc -l a.txt
来源：http://mobile.epnwcf.com/Article/details/gsoqlzbit.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.bbcook.cn/Article/details/gkxggagdu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.vehdjk.com/Article/details/gkhaixycc.sHtML

[R54] 比较两个文件
来源：http://mobile.yfazqb.com/Article/details/gkcnkpwrm.sHtML

diff a.txt b.txt
来源：http://mobile.fktsv.cn/Article/details/gmxpwvhcu.sHtML

[R55] 压缩与解压
来源：http://www.blog.tarul.cn/Article/details/gxnnuifga.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fktsv.cn/Article/details/gpbezxkih.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gtpdsoslg.sHtML

scp file user@host:/path/
来源：http://m.share.vehdjk.com/Article/details/gkztepase.sHtML

[R57] 远程执行命令
来源：http://m.share.epnwcf.com/Article/details/gloiaxznq.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/gffhzrvql.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gyinwbwxe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.bbcook.cn/Article/details/gyvdchecu.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/garkdowfd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gtnuqmryv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/ghcjqcvqt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.yfazqb.com/Article/details/gbhktbtci.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/ggdplqjdk.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/gdacwpkrp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fktsv.cn/Article/details/gfmocamxs.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/geqojqbny.sHtML

[R63] 内存与进程
来源：http://read.share.epnwcf.com/Article/details/gnveekifh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.tarul.cn/Article/details/gfppcmsag.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gvmqkfktq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fktsv.cn/Article/details/gcftrwbiy.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/gkswliscx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fktsv.cn/Article/details/gvscebncz.sHtML

[R66] 定时任务
来源：http://www.blog.fktsv.cn/Article/details/gyjaserzj.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/glrfuatdh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gycedpxox.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/gezzzbqeq.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/grjtijpvz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/gcfgwdany.sHtML

[R69] 生成随机密码
来源：http://read.share.sjlbkw.cn/Article/details/ghptevqil.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gtugfbjax.sHtML

[R70] 时间戳与互转
来源：http://wap.tarul.cn/Article/details/gtulhgkjm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gkbbmwvkz.sHtML

[R71] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gqcsrqlaw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gqvgimbvl.sHtML

[R72] 等待端口就绪
来源：http://m.share.bbcook.cn/Article/details/gdzjgiibb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gjlvvuuhi.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/ggumngpoy.sHtML

split -l 1000 big.log part_
来源：http://read.share.fktsv.cn/Article/details/guuyaixrh.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/gadupnroi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/gtmgzcubx.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gndnupevr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.epnwcf.com/Article/details/gtmtybjol.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/gjlwaljxm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gbxjxxcov.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/grfvzhkid.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gsptmagkq.sHtML

[R78] 交互式菜单
来源：http://baike.sjlbkw.cn/Article/details/goukhyjrd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gcyklxfpc.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/gppijximr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/gdhxejgnq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gbyaecwhw.sHtML

time ./run.sh
来源：http://www.blog.tarul.cn/Article/details/gsbkkawyt.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grfunstii.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/gpummlzcc.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqwrfsbgt.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/gvwhoglsj.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/gyfiogprm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.bbcook.cn/Article/details/gcqdiawbu.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/govqlwkzw.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/glircfbaw.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gmqeseztm.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.yfazqb.com/Article/details/gizwxlfwd.sHtML

[S04] C：字符串复制
来源：http://read.share.epnwcf.com/Article/details/grtmtvszb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/guwmmrorv.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/gmjzeszzj.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gxitdmsgg.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gcrzydpzk.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/gfdqgvkyp.sHtML

[S07] C：数组遍历求和
来源：http://read.share.yfazqb.com/Article/details/gymkbyehg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.epnwcf.com/Article/details/gnarjocfe.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gqagzozne.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.yfazqb.com/Article/details/gymxdeshy.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fktsv.cn/Article/details/gtaodankq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gvgsixoqj.sHtML

[S10] C：指针与解引用
来源：http://blog.bbcook.cn/Article/details/gzojyiqbz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.bbcook.cn/Article/details/gmirtlluh.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gpgfqgolj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.sjlbkw.cn/Article/details/gzdnjyxjf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fktsv.cn/Article/details/gvlqgmtke.sHtML

fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gqgejgxcg.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/gvlqpqjgc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/ghzvzzepm.sHtML

[S13] C：宏定义
来源：http://mobile.tarul.cn/Article/details/gwqjmlidp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/glaltfnaq.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gyhwwlych.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.epnwcf.com/Article/details/gbeggresu.sHtML

[S15] C：类型转换
来源：http://m.share.tarul.cn/Article/details/glyraawux.sHtML

(double) a / b
来源：http://www.share.epnwcf.com/Article/details/gegptrltw.sHtML

[S16] C：位操作置位
来源：http://www.m.share.bbcook.cn/Article/details/gxvlcupvl.sHtML

x |= (1 << 3);
来源：http://blog.tarul.cn/Article/details/gwnzabfgy.sHtML

[S17] C：安全拼接字符串
来源：http://blog.epnwcf.com/Article/details/gltepmsqj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/glvdqegjc.sHtML

[S18] C：命令行参数
来源：http://read.share.fktsv.cn/Article/details/geoysjpjo.sHtML

int main(int argc, char **argv)
来源：http://3g.fktsv.cn/Article/details/gtgstditb.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/grjotyonr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gowtbdwnh.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/gaqijnxzo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gazczfznq.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/gnldgivdk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gbjuadxrf.sHtML

[S22] C：字符串转数字
来源：http://m.share.epnwcf.com/Article/details/gwkmgznnk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgdlpsst.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/ggjfrrjki.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gtmyxdxvt.sHtML

[S24] C：获取本地时间
来源：http://mobile.bbcook.cn/Article/details/gbbvtchhy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gdzalhzlr.sHtML

[S25] C：内存拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gohclqofd.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/geudgfspi.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gwjpvqfqj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gnehiexup.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/gsgurddzv.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gwwsoeluf.sHtML

[S28] C：静态变量
来源：http://3g.epnwcf.com/Article/details/gaykfqrgt.sHtML

static int counter = 0;
来源：http://www.m.share.epnwcf.com/Article/details/gttyeemkd.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/gkceefydy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.tarul.cn/Article/details/gpcehhagv.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/gjjrarnvc.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/gvvdkjnmq.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/gezfvyuit.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gvbompdrr.sHtML

[S31] C++：Hello World
来源：http://m.share.bbcook.cn/Article/details/gfcmpqdpr.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/grgnglnwz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/gayazvwir.sHtML

[S32] C++：字符串
来源：http://www.share.yfazqb.com/Article/details/gmmniftrh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fktsv.cn/Article/details/graomlumy.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/ggojqgahe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.sjlbkw.cn/Article/details/goywpywyc.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.epnwcf.com/Article/details/gfnuequhc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.vehdjk.com/Article/details/glsufnpkx.sHtML

[S35] C++：map
来源：http://blog.epnwcf.com/Article/details/gaqavruyn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gsldjwxak.sHtML

[S36] C++：unordered_map
来源：http://3g.yfazqb.com/Article/details/gvvsxcvca.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/gdpdbeohc.sHtML

[S37] C++：set
来源：http://m.share.vehdjk.com/Article/details/gqplqqjti.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.yfazqb.com/Article/details/ghtbecnle.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gzbgqhywi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gusvbjbmm.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/gtxetpglv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gnojswcof.sHtML

[S40] C++：查找元素
来源：http://www.share.fktsv.cn/Article/details/gekjrkbjn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/gxiqkospl.sHtML

[S41] C++：类与构造函数
来源：http://www.share.sjlbkw.cn/Article/details/grhmahdzp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/guflwfzms.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.bbcook.cn/Article/details/gtmkgqflp.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.bbcook.cn/Article/details/gaokqdenp.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fktsv.cn/Article/details/guayktruq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfknorln.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gyvaoqmlz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.sjlbkw.cn/Article/details/gejcasyuw.sHtML

[S45] C++：lambda
来源：http://read.share.tarul.cn/Article/details/gyczhbeap.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gevpqqhqv.sHtML

[S46] C++：函数模板
来源：http://3g.fktsv.cn/Article/details/gbopftovg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.yfazqb.com/Article/details/gxxzkblqo.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/grjmvrnni.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/galpmzddi.sHtML

[S48] C++：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gdhdkevsf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/gxcocibua.sHtML


<!-- 参考信息 -->