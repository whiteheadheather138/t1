代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvdfsohu.sHtML

[Q75] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gsaonxrkt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gthrtyrep.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fktsv.cn/Article/details/gqrfsrias.sHtML

[Q76] 按天统计
来源：http://read.share.sjlbkw.cn/Article/details/grxrnluok.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fktsv.cn/Article/details/gjtzzibbs.sHtML

[Q77] 时间加减
来源：http://mobile.sjlbkw.cn/Article/details/gdnybouyb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fktsv.cn/Article/details/gnsxamzfk.sHtML

[Q78] 当前时间
来源：http://www.blog.yfazqb.com/Article/details/ggxqeydyb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/geaztisot.sHtML

[Q79] 字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gslfacrju.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.vehdjk.com/Article/details/gboeojedz.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/gyipioqta.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gmbrzijfp.sHtML

[Q81] 字符串替换
来源：http://3g.epnwcf.com/Article/details/ggbtrsoea.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gqkjulocx.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gzibcbqdz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gbqwgfkzj.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gffcxibhu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/ggjqsuvqd.sHtML

[Q84] 去除首尾空格
来源：http://wap.epnwcf.com/Article/details/guoqelozf.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/goqfkloxh.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/ggardjoet.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.sjlbkw.cn/Article/details/gjjbnvlof.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.epnwcf.com/Article/details/gwxqrnpdp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.vehdjk.com/Article/details/gmvywchrv.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.sjlbkw.cn/Article/details/ghwyhkpzx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gtnpnezvn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.vehdjk.com/Article/details/gyupceesd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/gthawstbp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.yfazqb.com/Article/details/gbymtmrir.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/gsaltapot.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/gtpcieoff.sHtML

[Q90] 生成序号列
来源：http://blog.tarul.cn/Article/details/gcljyvepz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.vehdjk.com/Article/details/gemtfrenb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcsojgsyk.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/gibyfzqvi.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvgjgkzvj.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gnhrnmiej.sHtML

#!/usr/bin/env bash
来源：http://baike.tarul.cn/Article/details/gcolmgrba.sHtML

set -euo pipefail
来源：http://m.share.bbcook.cn/Article/details/gbqxkoynz.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gqzgcrors.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.tarul.cn/Article/details/ggyvbszjy.sHtML

[R03] 只读变量
来源：http://mobile.vehdjk.com/Article/details/gdvpyoehh.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gaaitbsbl.sHtML

[R04] 位置参数
来源：http://wap.fktsv.cn/Article/details/gdgzpvyam.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.vehdjk.com/Article/details/gdbsfdnzv.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwajtosk.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/gmjuwcnel.sHtML

[R06] 判断命令是否存在
来源：http://blog.tarul.cn/Article/details/gactkrcwy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/glveremna.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/ggeqdkfdy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fktsv.cn/Article/details/gggjomihb.sHtML

[R08] 数值比较
来源：http://mobile.tarul.cn/Article/details/gttkwewfb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gsjndcxsa.sHtML

[R09] 字符串比较
来源：http://baike.tarul.cn/Article/details/ghposmbtx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.sjlbkw.cn/Article/details/gvyoeyoto.sHtML

[R10] 正则匹配
来源：http://mobile.sjlbkw.cn/Article/details/gqlqtbcov.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gzydzvayw.sHtML

[R11] case 多分支
来源：http://blog.fktsv.cn/Article/details/gdurujohq.sHtML

case "$1" in
来源：http://3g.fktsv.cn/Article/details/gnfxpkrkj.sHtML

start) echo "启动" ;;
来源：http://baike.vehdjk.com/Article/details/guviexthc.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fktsv.cn/Article/details/ginknbzps.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/gmqsikpuk.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/gjrpspntr.sHtML

[R12] for 遍历文件
来源：http://blog.vehdjk.com/Article/details/gpndxmkyr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/gkrqveftf.sHtML

[R13] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/giolsnzzl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/ggfdfutqx.sHtML

[R14] C 风格 for
来源：http://m.share.epnwcf.com/Article/details/gegnibkfa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/glbvvyzkk.sHtML

[R15] while 逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gvvhjuthr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/gifctsmiq.sHtML

[R16] until 等待条件
来源：http://m.share.epnwcf.com/Article/details/gpyhkyfkp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/geximlyuk.sHtML

[R17] 数组定义与取值
来源：http://mobile.yfazqb.com/Article/details/glkrswqix.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gizwkvcax.sHtML

[R18] 遍历数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkhoacla.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/glybtbiaa.sHtML

[R19] 数组长度
来源：http://www.share.tarul.cn/Article/details/gwojwsoxw.sHtML

echo "${#arr[@]}"
来源：http://mobile.bbcook.cn/Article/details/gapgxsgps.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/gtqgeengs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gizmudogz.sHtML

[R21] 字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gzgiakrep.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gninvgttb.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gbjbnsarv.sHtML

echo "${s:0:5}"
来源：http://3g.bbcook.cn/Article/details/gwlmuszjk.sHtML

[R23] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gwvabiohm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fktsv.cn/Article/details/ggpfyhdyo.sHtML

[R24] 大小写转换
来源：http://3g.tarul.cn/Article/details/guceznigw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/gepyhkyvd.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/gmscveiwa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.vehdjk.com/Article/details/gvihaljdp.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/ggunjbnmj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.sjlbkw.cn/Article/details/ggjkvfeab.sHtML

[R27] 算术展开
来源：http://mobile.sjlbkw.cn/Article/details/gqlwrbtqs.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.yfazqb.com/Article/details/gjquzaoav.sHtML

[R28] 浮点运算
来源：http://wap.yfazqb.com/Article/details/gpbxexbrv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.tarul.cn/Article/details/guesartki.sHtML

[R29] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gupdenlwc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/gygoifxyt.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/gfnivwslr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/gbpksngkx.sHtML

[R31] 局部变量
来源：http://3g.tarul.cn/Article/details/gnsbulfde.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/ghikdcrml.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/ggvblevst.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gzqcysirs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/gctczkyhi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gsvwnliqn.sHtML

[R34] 退出时清理
来源：http://baike.tarul.cn/Article/details/gggjabfwj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gfwmpozfv.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/gyoplarhm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/gvqoikoca.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/guxxbbcgp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/gzhysgojy.sHtML

[R37] 把输出赋给变量
来源：http://wap.bbcook.cn/Article/details/gvzjcsvbb.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwemjfdsy.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gsctloijz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.tarul.cn/Article/details/gpxfawhbz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/gxqpctwnt.sHtML

cmd > out.log 2>&1
来源：http://read.share.epnwcf.com/Article/details/gxegvtewf.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/gyezocuiw.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gqwkscito.sHtML

[R41] 丢弃输出
来源：http://blog.bbcook.cn/Article/details/gtrcqbaqo.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/geuystnbe.sHtML

[R42] 输入重定向
来源：http://www.m.share.sjlbkw.cn/Article/details/gqknxwjho.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gqevnepwe.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gpvztazkr.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gqtwfqrpq.sHtML

[R44] 按修改时间查找
来源：http://mobile.sjlbkw.cn/Article/details/gkxacwsnh.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gtbhkmchu.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/gfkzvjqyy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/grasvwpfw.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fktsv.cn/Article/details/gdhxnswja.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/glqhsfjlt.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/gawicfnki.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/ggirqqdrx.sHtML

[R48] awk 取指定列
来源：http://read.share.bbcook.cn/Article/details/gdoimsvtp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/ghykgrcxu.sHtML

[R49] awk 带条件
来源：http://m.share.tarul.cn/Article/details/gmazgzkff.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fktsv.cn/Article/details/gpbdlvyiu.sHtML

[R50] awk 求和
来源：http://wap.bbcook.cn/Article/details/gvtouqhat.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fktsv.cn/Article/details/gboibenyf.sHtML

[R51] 排序去重取前几
来源：http://blog.epnwcf.com/Article/details/gwmaqcslr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fktsv.cn/Article/details/ggciplcyy.sHtML

[R52] 统计行数
来源：http://baike.sjlbkw.cn/Article/details/glnzmfveh.sHtML

wc -l a.txt
来源：http://www.share.fktsv.cn/Article/details/ggddhyrnz.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.sjlbkw.cn/Article/details/gcjiwrqba.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.bbcook.cn/Article/details/gocgdognl.sHtML

[R54] 比较两个文件
来源：http://blog.tarul.cn/Article/details/gsmkssdaj.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/gqpamyzae.sHtML

[R55] 压缩与解压
来源：http://www.share.sjlbkw.cn/Article/details/gvwazauwo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fktsv.cn/Article/details/guwjkzhzv.sHtML

[R56] 远程拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gbhuivdez.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gujgpvwkt.sHtML

[R57] 远程执行命令
来源：http://read.share.fktsv.cn/Article/details/gjfghdror.sHtML

ssh user@host 'uptime'
来源：http://www.blog.sjlbkw.cn/Article/details/gauonvkxc.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/gouvvdzfb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.bbcook.cn/Article/details/glyeoehez.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gdnitefen.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuxcuupi.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gzewbwyhg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.yfazqb.com/Article/details/gyqldjihm.sHtML

[R61] 磁盘占用
来源：http://blog.yfazqb.com/Article/details/gbzbylrha.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/ghypnvjbf.sHtML

[R62] 找最占空间的文件
来源：http://3g.sjlbkw.cn/Article/details/gzbytihdm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.yfazqb.com/Article/details/gxjkkdivo.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/gkpgtbuqv.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fktsv.cn/Article/details/galdtqdoq.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/gzkprvdkv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.bbcook.cn/Article/details/gmincngaj.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/ghdskjmah.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gtcdxdpyv.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/guekyammo.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/gakllszfi.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gahdnyhxg.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/gvzvcsbhi.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gdvieiaor.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.vehdjk.com/Article/details/gdrbkubyt.sHtML

[R69] 生成随机密码
来源：http://read.share.yfazqb.com/Article/details/gtyllnosm.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fktsv.cn/Article/details/gqifjwzlw.sHtML

[R70] 时间戳与互转
来源：http://read.share.fktsv.cn/Article/details/gdglfwqyk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/giyeaekgn.sHtML

[R71] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gnvsvnrvy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gdrexvjlt.sHtML

[R72] 等待端口就绪
来源：http://www.share.sjlbkw.cn/Article/details/gfetifogg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gxakwqcfg.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/gntdthhve.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/getulxtck.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/gtygzqhsg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.vehdjk.com/Article/details/ginhwonbc.sHtML

[R75] 导出环境变量
来源：http://blog.bbcook.cn/Article/details/gebiqehsm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.epnwcf.com/Article/details/gmlmsikln.sHtML

[R76] 使用临时文件
来源：http://m.share.fktsv.cn/Article/details/gktxjygyc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gtfbqlgna.sHtML

[R77] 读取用户输入
来源：http://blog.tarul.cn/Article/details/gvbauujds.sHtML

read -rp "请输入: " ans
来源：http://wap.fktsv.cn/Article/details/gxmbtlaqt.sHtML

[R78] 交互式菜单
来源：http://3g.yfazqb.com/Article/details/gecvmddso.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.sjlbkw.cn/Article/details/gouhpmwwg.sHtML

[R79] 解析命令行选项
来源：http://read.share.bbcook.cn/Article/details/gzusnhlmj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gnahgmbsy.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/ggkivlllj.sHtML

time ./run.sh
来源：http://www.m.share.vehdjk.com/Article/details/gjquhgayx.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gtjdjpyas.sHtML

S. C / C++ 专题
来源：http://read.share.fktsv.cn/Article/details/grtiqptjh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gyrhkqmwp.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/gkaemseni.sHtML

#include <stdio.h>
来源：http://3g.fktsv.cn/Article/details/gkzezuqbb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gsowbxvbt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/geujaqdbm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.epnwcf.com/Article/details/gktiqabar.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gvympktzl.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/gavptunvp.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/ggphgyqps.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/gzrmxzoik.sHtML

[S05] C：字符串长度
来源：http://baike.sjlbkw.cn/Article/details/ggdfowpru.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gxhviqlzu.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gkxucrekb.sHtML

strcmp(a, b) == 0
来源：http://3g.epnwcf.com/Article/details/gjcptgwbz.sHtML

[S07] C：数组遍历求和
来源：http://baike.vehdjk.com/Article/details/ghpwczjzk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.tarul.cn/Article/details/gksaecqez.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.sjlbkw.cn/Article/details/gfigaaate.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.bbcook.cn/Article/details/gpobzmmnm.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/gdwfkayet.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gvtkjcfpl.sHtML

[S10] C：指针与解引用
来源：http://www.blog.bbcook.cn/Article/details/gfscafnwz.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fktsv.cn/Article/details/ghnwwnoux.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gdvirszes.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gcikwwxvz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.epnwcf.com/Article/details/gygqpulpb.sHtML

fclose(f);
来源：http://blog.vehdjk.com/Article/details/gmkftwkoo.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/gjetgtnvt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gjxgwsqpt.sHtML

[S13] C：宏定义
来源：http://read.share.fktsv.cn/Article/details/gqxmyqbal.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.vehdjk.com/Article/details/gluukyofp.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/geirnpxrk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.vehdjk.com/Article/details/gtskiuzie.sHtML

[S15] C：类型转换
来源：http://baike.epnwcf.com/Article/details/ggneqekfc.sHtML

(double) a / b
来源：http://www.m.share.tarul.cn/Article/details/gdzhpqbfx.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/gbqbuavbk.sHtML

x |= (1 << 3);
来源：http://blog.epnwcf.com/Article/details/grtduuqpa.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gkxdhrvbt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gcpqlxiwd.sHtML

[S18] C：命令行参数
来源：http://wap.epnwcf.com/Article/details/gtsdcngkh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/giyhxvirm.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/grysvuhoz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gzsfigrbl.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gggowsfpk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gmdaphdbv.sHtML

[S21] C：字符类别判断
来源：http://www.share.vehdjk.com/Article/details/gucurfdzm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.sjlbkw.cn/Article/details/glofubjwt.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gduiubdpr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/gzuirwbwx.sHtML

[S23] C：随机数
来源：http://www.blog.yfazqb.com/Article/details/gnwwlxezu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gscftrijy.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/gnshdbmtz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fktsv.cn/Article/details/geifroxor.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/gieivndnv.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gqyoddfuz.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/gjmrmkcie.sHtML

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gmjrsasfc.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/gobhecmpt.sHtML

const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/glzallpya.sHtML

[S28] C：静态变量
来源：http://www.blog.yfazqb.com/Article/details/gexnopmuw.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/gvvdmqgwr.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/grbtaaxni.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/gkynwhgzu.sHtML

[S30] C：头文件保护
来源：http://read.share.vehdjk.com/Article/details/gxgysnlvx.sHtML

#ifndef X_H
来源：http://www.blog.vehdjk.com/Article/details/gvwdmjepv.sHtML

#define X_H
来源：http://blog.bbcook.cn/Article/details/gbxqpjyqt.sHtML

#endif
来源：http://mobile.epnwcf.com/Article/details/gjosgqgam.sHtML

[S31] C++：Hello World
来源：http://wap.yfazqb.com/Article/details/gwjhrqusu.sHtML

#include <iostream>
来源：http://www.share.sjlbkw.cn/Article/details/gafjzqhml.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gwcavgiaf.sHtML

[S32] C++：字符串
来源：http://www.m.share.vehdjk.com/Article/details/gpkntjliy.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fktsv.cn/Article/details/gendaadbl.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/gygpcdyoh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gjhbbksut.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/gkdfezgxu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/gxizxjdhi.sHtML

[S35] C++：map
来源：http://read.share.epnwcf.com/Article/details/gkdxmjxki.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/griwqdknh.sHtML

[S36] C++：unordered_map
来源：http://www.blog.tarul.cn/Article/details/ghiumbqdt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/ghuwwtyat.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/gfrxuphmy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fktsv.cn/Article/details/gctqheach.sHtML

[S38] C++：排序
来源：http://mobile.bbcook.cn/Article/details/gfsvypopi.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gammukvqr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gjzjtsjgz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.yfazqb.com/Article/details/gmrrltncu.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/gvnnyffxp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gnuhmkpdh.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gbnsrjwoh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/gvfusgnuu.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.bbcook.cn/Article/details/gvyarwtim.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.yfazqb.com/Article/details/gmuaoycno.sHtML

[S43] C++：智能指针
来源：http://wap.fktsv.cn/Article/details/gwkjskrfi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/gcjxbngwi.sHtML

[S44] C++：引用传参
来源：http://www.blog.tarul.cn/Article/details/gpxmnidou.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/gzewjzfhi.sHtML


<!-- 参考信息 -->