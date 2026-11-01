代发 wailian999

[Q76] 按天统计
来源：http://www.blog.epnwcf.com/Article/details/gdlqrtqsf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.vehdjk.com/Article/details/gnbtnocnl.sHtML

[Q77] 时间加减
来源：http://read.share.sjlbkw.cn/Article/details/gxptscsdv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gjnrebwyu.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/gzsxizsjj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.epnwcf.com/Article/details/gszgjociz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/gfburaflj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/guzhgphal.sHtML

[Q80] 字符串截取
来源：http://3g.bbcook.cn/Article/details/gsgkiuadb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gstmiitra.sHtML

[Q81] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gemcooano.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.vehdjk.com/Article/details/gpahodhqm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.tarul.cn/Article/details/gufutmxhz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gvdccwrth.sHtML

[Q83] 大小写转换
来源：http://baike.fktsv.cn/Article/details/glngzpgje.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gwixhriaz.sHtML

[Q84] 去除首尾空格
来源：http://www.share.bbcook.cn/Article/details/gxaaegfvt.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gfqxsntik.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gjavsgspm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fktsv.cn/Article/details/golbehdpo.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fktsv.cn/Article/details/gyahgecar.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.vehdjk.com/Article/details/gyiaqwxee.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fktsv.cn/Article/details/gkiimymmw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.yfazqb.com/Article/details/goqnfifto.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.yfazqb.com/Article/details/gdvovzkjc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.tarul.cn/Article/details/gxizpqzha.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fktsv.cn/Article/details/gmoelpuvc.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fktsv.cn/Article/details/ggiiqqpnj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/gwuntbdvn.sHtML

[Q90] 生成序号列
来源：http://www.blog.tarul.cn/Article/details/gorlsfflf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/goyntllvm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfcxakdbw.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/gdbampuvb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtsvxyryx.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gnuvmiwif.sHtML

#!/usr/bin/env bash
来源：http://wap.bbcook.cn/Article/details/gmoafflfi.sHtML

set -euo pipefail
来源：http://blog.vehdjk.com/Article/details/gjzsmtdrg.sHtML

[R02] 变量赋值与使用
来源：http://www.share.tarul.cn/Article/details/gxeyxhiyd.sHtML

name="Tom"; echo "$name"
来源：http://read.share.yfazqb.com/Article/details/gvukbjsdz.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/gjplbazba.sHtML

readonly PI=3.14
来源：http://read.share.yfazqb.com/Article/details/glaexshgw.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/gavrwfsej.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fktsv.cn/Article/details/gnfjfzwhg.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/gxjeyogck.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/gphfyxqvw.sHtML

[R06] 判断命令是否存在
来源：http://m.share.vehdjk.com/Article/details/gqdjyiqdh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gcnrgwxbq.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/gmcdqyirs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/gutvyiwit.sHtML

[R08] 数值比较
来源：http://m.share.sjlbkw.cn/Article/details/gqqkctejw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.vehdjk.com/Article/details/gqvgdsqgc.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gojkrdzbw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.vehdjk.com/Article/details/gtxlibyeu.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/gkszjuwha.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gxczxhkdx.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/giqcbzzuz.sHtML

case "$1" in
来源：http://wap.epnwcf.com/Article/details/gufclpdcq.sHtML

start) echo "启动" ;;
来源：http://wap.fktsv.cn/Article/details/glxcqiksh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.vehdjk.com/Article/details/gukamqzwd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gmusbyazv.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gbgsbvmed.sHtML

[R12] for 遍历文件
来源：http://blog.yfazqb.com/Article/details/gitomuwwl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gveuxredq.sHtML

[R13] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/gmfemobuy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gipyiodry.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gprgnhnvq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gluwnuldn.sHtML

[R15] while 逐行读文件
来源：http://3g.fktsv.cn/Article/details/ghaglghzu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gitqumjnf.sHtML

[R16] until 等待条件
来源：http://www.share.fktsv.cn/Article/details/gjagualbx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gkmlqvymy.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/gnafwtiyd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/gvubnejnb.sHtML

[R18] 遍历数组
来源：http://baike.epnwcf.com/Article/details/gkdqohtyd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.yfazqb.com/Article/details/gjjijqyio.sHtML

[R19] 数组长度
来源：http://3g.epnwcf.com/Article/details/gazndneye.sHtML

echo "${#arr[@]}"
来源：http://m.share.vehdjk.com/Article/details/gmdtgiixf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.vehdjk.com/Article/details/gtkupznxw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.sjlbkw.cn/Article/details/gaouvnqrn.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gdxltufye.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gfmcbdedu.sHtML

[R22] 截取子串
来源：http://mobile.epnwcf.com/Article/details/ggtvkyxan.sHtML

echo "${s:0:5}"
来源：http://www.share.bbcook.cn/Article/details/gzvlowilx.sHtML

[R23] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gxyxowwfe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.yfazqb.com/Article/details/guzjohajf.sHtML

[R24] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gfdvcmbba.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gxvddazoj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fktsv.cn/Article/details/guttnckdg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.epnwcf.com/Article/details/gwxmtiztj.sHtML

[R26] 命令替换
来源：http://www.share.yfazqb.com/Article/details/gqefdfbvx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.sjlbkw.cn/Article/details/gbonkajak.sHtML

[R27] 算术展开
来源：http://read.share.vehdjk.com/Article/details/gwhpjaqgt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.sjlbkw.cn/Article/details/gywqqodll.sHtML

[R28] 浮点运算
来源：http://blog.epnwcf.com/Article/details/getrhzvoj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.yfazqb.com/Article/details/gyqengyom.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gvxrumqoz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gafxwntpm.sHtML

[R30] 函数返回状态码
来源：http://wap.fktsv.cn/Article/details/gobgvcdkg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.epnwcf.com/Article/details/gtkokvmnw.sHtML

[R31] 局部变量
来源：http://www.share.fktsv.cn/Article/details/ggcmphxcw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fktsv.cn/Article/details/gkizuoann.sHtML

[R32] 参数个数校验
来源：http://blog.tarul.cn/Article/details/gakyvvagb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gqxynffvl.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.sjlbkw.cn/Article/details/gcfktkpua.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/gjuwtirel.sHtML

[R34] 退出时清理
来源：http://blog.sjlbkw.cn/Article/details/guopzttzx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gdrspgkgn.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gufjntncv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.yfazqb.com/Article/details/gvxbzlbxl.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.vehdjk.com/Article/details/gdubmabmm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gkqznexvu.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/gyciddzrj.sHtML

files=$(ls -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyocqifxn.sHtML

[R38] 管道串联
来源：http://www.share.bbcook.cn/Article/details/goybcfvpm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.bbcook.cn/Article/details/gyufygabw.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fktsv.cn/Article/details/gkzivrths.sHtML

cmd > out.log 2>&1
来源：http://m.share.bbcook.cn/Article/details/gewmhmxep.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/gtgjovjsg.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/gmqtahgrm.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fktsv.cn/Article/details/gehgtdzta.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gcszwbkwm.sHtML

[R42] 输入重定向
来源：http://www.blog.fktsv.cn/Article/details/gnirvqbqd.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/glzhmpwjt.sHtML

[R43] 按名字查找文件
来源：http://3g.bbcook.cn/Article/details/gerpftrkt.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/gndyatwrc.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/ghjsashbi.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gsivzidpv.sHtML

[R45] 批量删除
来源：http://baike.yfazqb.com/Article/details/gidfosxsr.sHtML

find . -name "*.tmp" -delete
来源：http://blog.bbcook.cn/Article/details/gckhllxxg.sHtML

[R46] 递归替换文件内容
来源：http://wap.tarul.cn/Article/details/ghcnjlplg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/grrdbtyus.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/gvyhbjmvi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.yfazqb.com/Article/details/gnyrrmlfe.sHtML

[R48] awk 取指定列
来源：http://www.blog.tarul.cn/Article/details/gzabobqfr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.vehdjk.com/Article/details/grurfzbps.sHtML

[R49] awk 带条件
来源：http://www.blog.sjlbkw.cn/Article/details/gtnpojbdr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.epnwcf.com/Article/details/gocsckdmj.sHtML

[R50] awk 求和
来源：http://3g.epnwcf.com/Article/details/gmmlseegc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/ginllvinx.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gxdlybjph.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/gmtlnzale.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gyyviffha.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gxptqdpug.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.epnwcf.com/Article/details/gjvuqrmlb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/gvjoaftch.sHtML

[R54] 比较两个文件
来源：http://3g.sjlbkw.cn/Article/details/gremakmbb.sHtML

diff a.txt b.txt
来源：http://www.m.share.vehdjk.com/Article/details/gufagytdh.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/gnaayhuxw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.sjlbkw.cn/Article/details/gzbipybhp.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/gzszebglr.sHtML

scp file user@host:/path/
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpdqyyec.sHtML

[R57] 远程执行命令
来源：http://www.blog.bbcook.cn/Article/details/gqzetubey.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/gfpmdhraw.sHtML

[R58] 下载文件
来源：http://read.share.epnwcf.com/Article/details/gvyhmutxs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.yfazqb.com/Article/details/gpxvzyfhc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/ghhwgxkft.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/ghlnektjq.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gxyltrexa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/gvzopudze.sHtML

[R61] 磁盘占用
来源：http://m.share.tarul.cn/Article/details/gqilthtpd.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gdtnuuzxo.sHtML

[R62] 找最占空间的文件
来源：http://3g.bbcook.cn/Article/details/gusrnfjxo.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/gqvancqow.sHtML

[R63] 内存与进程
来源：http://blog.bbcook.cn/Article/details/gwayhgmdy.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fktsv.cn/Article/details/gcwxetfmf.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gxruvhldl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gyfqcrcgx.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/gkafsrwhh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.tarul.cn/Article/details/gsfkydlqh.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/gcfgepzvb.sHtML

crontab -e;  crontab -l
来源：http://m.share.sjlbkw.cn/Article/details/gvlpuqhip.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gqilaaptb.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/gavvvsetm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fktsv.cn/Article/details/gvgwrctst.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/gaaxjgdyw.sHtML

[R69] 生成随机密码
来源：http://www.blog.fktsv.cn/Article/details/gncfqlkmq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gyxipzdhl.sHtML

[R70] 时间戳与互转
来源：http://blog.epnwcf.com/Article/details/ghcuopxsk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.yfazqb.com/Article/details/gywhwmxhk.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gfdmbjehz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/giepruekh.sHtML

[R72] 等待端口就绪
来源：http://mobile.fktsv.cn/Article/details/gpfxqcrmo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gmaboknnp.sHtML

[R73] 分割大日志
来源：http://3g.yfazqb.com/Article/details/glqkngwoa.sHtML

split -l 1000 big.log part_
来源：http://read.share.vehdjk.com/Article/details/gupvlqgyw.sHtML

[R74] 批量重命名
来源：http://www.blog.fktsv.cn/Article/details/gckknlimj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gessejvrr.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gwlqakagj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/gepspoujd.sHtML

[R76] 使用临时文件
来源：http://mobile.fktsv.cn/Article/details/goukqiqwo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/goexsuaoa.sHtML

[R77] 读取用户输入
来源：http://blog.tarul.cn/Article/details/gaszudrmh.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/gsaqqisbu.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gphubzxnc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.yfazqb.com/Article/details/gwceaopsb.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/ghwjarits.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fktsv.cn/Article/details/gefosgmmb.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.epnwcf.com/Article/details/gyalxqkvw.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/gpcilziam.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gcfcoowfw.sHtML

S. C / C++ 专题
来源：http://blog.epnwcf.com/Article/details/gyzzqkupa.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/guxwzrcht.sHtML

[S01] C：Hello World
来源：http://blog.vehdjk.com/Article/details/gnvfkfebn.sHtML

#include <stdio.h>
来源：http://blog.sjlbkw.cn/Article/details/gyzeugjir.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/gdbclmasz.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gmqhodaof.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.sjlbkw.cn/Article/details/gbflabpus.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gfqnuauvg.sHtML

int x; scanf("%d", &x);
来源：http://3g.fktsv.cn/Article/details/gszqdeqbu.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/giuipfajo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gmldegjsp.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gatmdabqt.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/govmmfirk.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/ggvppkmxv.sHtML

strcmp(a, b) == 0
来源：http://wap.bbcook.cn/Article/details/gobyhyvxu.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gxjhrmcxq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/guvyyqmkt.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gsrjpsxav.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/gtqtugfba.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/gvekjlzrp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/gcsqdtinm.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gjzgytukp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.sjlbkw.cn/Article/details/gfmnclmgm.sHtML

[S11] C：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gnlpnygme.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/gdqnlwqdi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/gkoxesjij.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gbdpkwhpb.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/grbyhiphn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/gylcmskeh.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gfiapctob.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.yfazqb.com/Article/details/gbwpeazgh.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/gilxhlerr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gxdussisq.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/glsmedsfh.sHtML

(double) a / b
来源：http://www.share.sjlbkw.cn/Article/details/gukapzobx.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gcexylnxk.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/ggofmfdnh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gxqyvcdhf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.epnwcf.com/Article/details/gjhyvxzef.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gcteyvlfd.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/gfqusduqb.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/gidewynba.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gttbobtzb.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/guttakqfr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gmxcbyehd.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/ggydpncfb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/gprwjlcal.sHtML

[S22] C：字符串转数字
来源：http://www.share.epnwcf.com/Article/details/gurclmwnk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/gdyxedtrr.sHtML

[S23] C：随机数
来源：http://www.blog.vehdjk.com/Article/details/givfnadak.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/gqyfjgsaa.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/genniyubv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/goecjprgk.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/glzbmjxqy.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gyjkxorae.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/gfxncetzd.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/gklnbnjlb.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/gpzqrnpqg.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gyqzudxgb.sHtML

[S28] C：静态变量
来源：http://m.share.fktsv.cn/Article/details/gihyuqjme.sHtML

static int counter = 0;
来源：http://www.blog.yfazqb.com/Article/details/ggjnrzqjm.sHtML

[S29] C：变参函数
来源：http://mobile.fktsv.cn/Article/details/gzmkmqjob.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/gonhqtbdj.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/gsnfahbkl.sHtML

#ifndef X_H
来源：http://blog.fktsv.cn/Article/details/gohsbpgms.sHtML

#define X_H
来源：http://www.m.share.yfazqb.com/Article/details/gzejnvhgo.sHtML

#endif
来源：http://baike.epnwcf.com/Article/details/gvyuiului.sHtML

[S31] C++：Hello World
来源：http://m.share.vehdjk.com/Article/details/golpzeeat.sHtML

#include <iostream>
来源：http://blog.sjlbkw.cn/Article/details/ggjctomif.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.sjlbkw.cn/Article/details/gsxjuetnp.sHtML

[S32] C++：字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gxvbklgaq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.bbcook.cn/Article/details/ggsomrhht.sHtML

[S33] C++：vector 增删
来源：http://m.share.yfazqb.com/Article/details/govvewnaj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.yfazqb.com/Article/details/gpljmuevy.sHtML

[S34] C++：遍历 vector
来源：http://read.share.tarul.cn/Article/details/gaitlksqm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/gabatmuwn.sHtML

[S35] C++：map
来源：http://baike.vehdjk.com/Article/details/gtcdbhdus.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gkrmmiwlb.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/ggypifgxj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gjwlnqqqr.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/goakipdyp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/gtxongpuj.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/gwwkbrhzn.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.bbcook.cn/Article/details/gkafgzfsw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.vehdjk.com/Article/details/grdtksizz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.tarul.cn/Article/details/grxxlfrlo.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/gulgpihsi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.yfazqb.com/Article/details/gorkbplgr.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gczecabyd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.sjlbkw.cn/Article/details/gyclffqel.sHtML

[S42] C++：继承与虚函数
来源：http://wap.sjlbkw.cn/Article/details/gdgufdyqt.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gfktqrnno.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/gjgxvkuhd.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.bbcook.cn/Article/details/ghsqmveyu.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/gotlozxpn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/ghpkjeudq.sHtML

[S45] C++：lambda
来源：http://read.share.tarul.cn/Article/details/gsejcikig.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.sjlbkw.cn/Article/details/ggezojyop.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/ggkrbecqc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.epnwcf.com/Article/details/gaeeneffy.sHtML


<!-- 参考信息 -->