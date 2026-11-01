代发 wailian999

[Q78] 当前时间
来源：http://www.blog.tarul.cn/Article/details/gkydfzlov.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/guhlhrfoy.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/grdwgoixj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fktsv.cn/Article/details/gqwkahnqr.sHtML

[Q80] 字符串截取
来源：http://3g.sjlbkw.cn/Article/details/gmqiwyodh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.yfazqb.com/Article/details/gxxksvorw.sHtML

[Q81] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gtpxuzoov.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/gdvfguoop.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/grovqntww.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/geummkspp.sHtML

[Q83] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/ghigygazh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gibtqdsmp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.tarul.cn/Article/details/gumlzyasu.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/grttovqbp.sHtML

[Q85] 数值取整
来源：http://baike.fktsv.cn/Article/details/gdrypygmm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.vehdjk.com/Article/details/gxayrhfrn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.bbcook.cn/Article/details/gzgcqusro.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.yfazqb.com/Article/details/gwngsvifm.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fktsv.cn/Article/details/gjrlewzgn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.bbcook.cn/Article/details/gpniwraqt.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.sjlbkw.cn/Article/details/gxghuhuuj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fktsv.cn/Article/details/gduzznmum.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/gvxcpbums.sHtML

[Q89] 判断表是否存在
来源：http://baike.tarul.cn/Article/details/grtppdxkf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/gtoeiappm.sHtML

[Q90] 生成序号列
来源：http://mobile.tarul.cn/Article/details/gqcwfypzq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.epnwcf.com/Article/details/glcjqlinl.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ggigjxwad.sHtML

R. Bash 专题
来源：http://blog.fktsv.cn/Article/details/guwfmnegh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvtihykcn.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.tarul.cn/Article/details/gjpnemjid.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/gmajgwpou.sHtML

set -euo pipefail
来源：http://m.share.yfazqb.com/Article/details/ggmqzgjjy.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/gqcgrkpgi.sHtML

name="Tom"; echo "$name"
来源：http://blog.tarul.cn/Article/details/gyqfswvvj.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/goesceltw.sHtML

readonly PI=3.14
来源：http://www.share.fktsv.cn/Article/details/gvwworeip.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gubkzyayt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.epnwcf.com/Article/details/gpvhjpuyv.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gvmkbcops.sHtML

name="${1:-default}"
来源：http://www.m.share.tarul.cn/Article/details/gnrsfzpun.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gkeihsbdk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gjoqwxkpu.sHtML

[R07] if 判断文件
来源：http://www.share.sjlbkw.cn/Article/details/gucludvhl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gndxrwdcm.sHtML

[R08] 数值比较
来源：http://m.share.yfazqb.com/Article/details/gutligbrh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gocistebd.sHtML

[R09] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gxecowwnx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.tarul.cn/Article/details/gnohbderv.sHtML

[R10] 正则匹配
来源：http://mobile.vehdjk.com/Article/details/grqlalwvp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/gtzjrqqgs.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/giaxzsjil.sHtML

case "$1" in
来源：http://read.share.vehdjk.com/Article/details/gcztnygzp.sHtML

start) echo "启动" ;;
来源：http://m.share.epnwcf.com/Article/details/gikpvwlkz.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/gpbklqtwe.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/gksqiqbsh.sHtML

esac
来源：http://www.m.share.epnwcf.com/Article/details/gsqixnnwl.sHtML

[R12] for 遍历文件
来源：http://baike.epnwcf.com/Article/details/gdkyznirn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/gyxhrfhpm.sHtML

[R13] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhklmdix.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gqpvrtfuu.sHtML

[R14] C 风格 for
来源：http://wap.yfazqb.com/Article/details/gvemasafu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gdnyjgsth.sHtML

[R15] while 逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gljdatajl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/gxpyjeowk.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gpogfhhfr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/gwdikdfnn.sHtML

[R17] 数组定义与取值
来源：http://wap.tarul.cn/Article/details/gcxvnuusa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.vehdjk.com/Article/details/gftnzgzfs.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/gkoiqnotz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/gtlzomqgz.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/gkhpzvlvu.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gecvhjerb.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gxtakzlbk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/ghhmswxvj.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/guvabwgbs.sHtML

echo "${#s}"
来源：http://www.share.vehdjk.com/Article/details/gjvoicwxh.sHtML

[R22] 截取子串
来源：http://www.share.fktsv.cn/Article/details/ggvghyxci.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/gekdnwtls.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gjnbqqtmj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/gldnougsq.sHtML

[R24] 大小写转换
来源：http://blog.bbcook.cn/Article/details/ggvtzpybb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fktsv.cn/Article/details/ginhfzsws.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.tarul.cn/Article/details/gpamwhmlz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/gogjqjtrv.sHtML

[R26] 命令替换
来源：http://blog.yfazqb.com/Article/details/gytdgcids.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.yfazqb.com/Article/details/gflpksdoj.sHtML

[R27] 算术展开
来源：http://www.blog.sjlbkw.cn/Article/details/gcvdwlluc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.epnwcf.com/Article/details/gcuafpqer.sHtML

[R28] 浮点运算
来源：http://www.share.tarul.cn/Article/details/gygdysmod.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.sjlbkw.cn/Article/details/gsmtdmrun.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gllvvpkjg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.tarul.cn/Article/details/giyfjezok.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/ggpvmyejv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gurtqmxjj.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gkqkcxcaw.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gzczymyvy.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gsgiijjvi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gitpyxckj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.yfazqb.com/Article/details/gmvoqhidh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/gqxtcztkw.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/gjsikimrg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gasnyhnfq.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/ghkqtxtox.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/ghzbqccmj.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/ghwiehyth.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.sjlbkw.cn/Article/details/gvimwqskp.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fktsv.cn/Article/details/grppzrkkz.sHtML

files=$(ls -1)
来源：http://baike.sjlbkw.cn/Article/details/gpcoejivf.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gareswsrq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.bbcook.cn/Article/details/gazlzodne.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/ghgxanest.sHtML

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/gyxllxvnu.sHtML

[R40] 追加写日志
来源：http://read.share.sjlbkw.cn/Article/details/gbiuedxyk.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/gddtzedbw.sHtML

[R41] 丢弃输出
来源：http://www.m.share.vehdjk.com/Article/details/ggghxkipy.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/gyywhtaft.sHtML

[R42] 输入重定向
来源：http://read.share.sjlbkw.cn/Article/details/gxqcbbrpy.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/genlwubjm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.yfazqb.com/Article/details/guqiairtz.sHtML

find . -name "*.log" -type f
来源：http://baike.yfazqb.com/Article/details/gssnytsps.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gfwhbzihq.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gvuonacqo.sHtML

[R45] 批量删除
来源：http://www.blog.sjlbkw.cn/Article/details/gxzdidaqx.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fktsv.cn/Article/details/gotcrcwkl.sHtML

[R46] 递归替换文件内容
来源：http://read.share.bbcook.cn/Article/details/gxipgxqaw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.bbcook.cn/Article/details/gedjhuvqh.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/gsgentxky.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gthetgmhf.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/gvzliglit.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gerbgotil.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gwzovczsz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/gnkvkujmg.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gjrafgxwm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gelodebwy.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/givjnkvxq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/gxkpkemvb.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gzlutpvzw.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/gcgxpjnkd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/gfltzmfyp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.vehdjk.com/Article/details/gpemojalu.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gqluaxrre.sHtML

diff a.txt b.txt
来源：http://m.share.fktsv.cn/Article/details/gowwhtqky.sHtML

[R55] 压缩与解压
来源：http://mobile.yfazqb.com/Article/details/gehepmixu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/gtczlrdqy.sHtML

[R56] 远程拷贝
来源：http://m.share.tarul.cn/Article/details/gussqubdn.sHtML

scp file user@host:/path/
来源：http://www.m.share.bbcook.cn/Article/details/ghmduwmig.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/garvwwlzi.sHtML

ssh user@host 'uptime'
来源：http://3g.epnwcf.com/Article/details/glxmovjlw.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gobtwfmxz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gbhcybxuk.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gvphqwzeo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gojtaflwy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/ginezvdsp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/gaxobtgaj.sHtML

[R61] 磁盘占用
来源：http://www.share.fktsv.cn/Article/details/gjmmojdle.sHtML

df -h;  du -sh *
来源：http://blog.bbcook.cn/Article/details/gbscqloxf.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/gngziwqvy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.sjlbkw.cn/Article/details/gujevaxqa.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/gvthvhgid.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.vehdjk.com/Article/details/gqfpwhpte.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/gbbjmdfpv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.sjlbkw.cn/Article/details/gjrwwioef.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/gzvohjsyj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.vehdjk.com/Article/details/gjnpngaqv.sHtML

[R66] 定时任务
来源：http://m.share.vehdjk.com/Article/details/ghjuxrszd.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/gajaskwaq.sHtML

[R67] 生成随机十六进制串
来源：http://blog.tarul.cn/Article/details/gyhfpojrq.sHtML

openssl rand -hex 16
来源：http://www.share.sjlbkw.cn/Article/details/gfskjjfkv.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.tarul.cn/Article/details/gvuwgrtli.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.yfazqb.com/Article/details/gostdvfky.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/gafmonvel.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.sjlbkw.cn/Article/details/gmnvjucaq.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/ghklkvyln.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.epnwcf.com/Article/details/gqnqbovtv.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gcfpmbgys.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.yfazqb.com/Article/details/gcswhkkdn.sHtML

[R72] 等待端口就绪
来源：http://read.share.bbcook.cn/Article/details/gxjsqssqr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gyfxwixiw.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/gdmefnfqj.sHtML

split -l 1000 big.log part_
来源：http://mobile.bbcook.cn/Article/details/guwlptnle.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/gnlyguzxj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.vehdjk.com/Article/details/ghjpdfdne.sHtML

[R75] 导出环境变量
来源：http://www.blog.fktsv.cn/Article/details/gotkuxslx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/goeedvpkc.sHtML

[R76] 使用临时文件
来源：http://m.share.vehdjk.com/Article/details/ghmamtpng.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gzeuimvsj.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/gdgsuztlt.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/glvfdjhqc.sHtML

[R78] 交互式菜单
来源：http://mobile.yfazqb.com/Article/details/gtiklniug.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gbawxeviz.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gjzrpxada.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.sjlbkw.cn/Article/details/gxmizpzfp.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gbbqgamwn.sHtML

time ./run.sh
来源：http://m.share.bbcook.cn/Article/details/gcgufuaep.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwqchdtht.sHtML

S. C / C++ 专题
来源：http://mobile.bbcook.cn/Article/details/gxwqaslkl.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwmjfhlbe.sHtML

[S01] C：Hello World
来源：http://www.share.bbcook.cn/Article/details/gjekjzjlm.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gobyqqiit.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gtlqjctxh.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gnczghfji.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/gxxgnibpi.sHtML

[S03] C：读入整数
来源：http://mobile.fktsv.cn/Article/details/gbxxtjnix.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gnpfozwox.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/gffxwattf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.sjlbkw.cn/Article/details/gykbcawta.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/gryjlfbuq.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gmzftliht.sHtML

[S06] C：字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gflqthuqy.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/gtwfzssge.sHtML

[S07] C：数组遍历求和
来源：http://3g.vehdjk.com/Article/details/gqoxuuljy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/gnbjpkfbf.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.yfazqb.com/Article/details/ggxxdpxiu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/ggowiruti.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/gbjxuubcb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.vehdjk.com/Article/details/gofarggmn.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/grczcafvl.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fktsv.cn/Article/details/gioktqqwd.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gaupmaokg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.sjlbkw.cn/Article/details/gjivgwnte.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fktsv.cn/Article/details/gmbyklanq.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gqyxbpalr.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/gpxgtylta.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gypkvkiez.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/gowlofcsp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.vehdjk.com/Article/details/gdbuqzipl.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gslbwpvwu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gqxsdilik.sHtML

[S15] C：类型转换
来源：http://m.share.tarul.cn/Article/details/gbyhnhboq.sHtML

(double) a / b
来源：http://mobile.bbcook.cn/Article/details/gztfuxuaw.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gpdaufmpq.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gvecaaqmq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gpcyazarw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.yfazqb.com/Article/details/gwkhcruff.sHtML

[S18] C：命令行参数
来源：http://3g.epnwcf.com/Article/details/gudeqjvrw.sHtML

int main(int argc, char **argv)
来源：http://read.share.tarul.cn/Article/details/gpliydhav.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gazdyywkd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gaujgmzyw.sHtML

[S20] C：二分查找
来源：http://www.share.epnwcf.com/Article/details/gbumamunf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gsysrobfx.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gbpqldffz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/gjgwhckkn.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/gvqnpcuxj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.yfazqb.com/Article/details/gbxahdjvg.sHtML

[S23] C：随机数
来源：http://3g.bbcook.cn/Article/details/gfmwnjtfy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.bbcook.cn/Article/details/gpealspgd.sHtML

[S24] C：获取本地时间
来源：http://blog.yfazqb.com/Article/details/gjjgfoesh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/gocixipkn.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/gdgzzeabu.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gctykqdso.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/gulsscuby.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/gxrvwised.sHtML

[S27] C：定义常量
来源：http://mobile.sjlbkw.cn/Article/details/ghlvrzuow.sHtML

const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gfmdrequh.sHtML

[S28] C：静态变量
来源：http://wap.yfazqb.com/Article/details/gttrnncpv.sHtML

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/gwifrviaf.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/gudwgifbt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/glvgdgdod.sHtML

[S30] C：头文件保护
来源：http://www.share.tarul.cn/Article/details/gpgdjspbf.sHtML

#ifndef X_H
来源：http://www.blog.epnwcf.com/Article/details/gurkwhogy.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/gwxlmbabj.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/golxxdifs.sHtML

[S31] C++：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gxbfloket.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/guwxqeufk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/gbllaovsb.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/gkfniwrsp.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fktsv.cn/Article/details/gsbmmxytm.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.yfazqb.com/Article/details/gwkeqotqp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.vehdjk.com/Article/details/gazyjaoys.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gegietjfv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.epnwcf.com/Article/details/grvcqlvoh.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/goqqnhvpv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gurthrtuu.sHtML

[S36] C++：unordered_map
来源：http://mobile.fktsv.cn/Article/details/gtpnzmisn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/gplsrkspw.sHtML

[S37] C++：set
来源：http://read.share.fktsv.cn/Article/details/glbgevzyi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.bbcook.cn/Article/details/gieycwxox.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/gmixwmkci.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gurtuqipb.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/gtlhwfxfn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.vehdjk.com/Article/details/gwdvmhqje.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/gtpyfkrnv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.bbcook.cn/Article/details/gihbwomnq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.tarul.cn/Article/details/gahhcvjbg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.epnwcf.com/Article/details/giyerciit.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjmgejtj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.tarul.cn/Article/details/gidjztrub.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/gqdvvazgc.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.epnwcf.com/Article/details/gdlhuydds.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/gndftzonr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gqozvdicg.sHtML

[S45] C++：lambda
来源：http://www.blog.fktsv.cn/Article/details/gvbdtvrws.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.bbcook.cn/Article/details/glhpdryxt.sHtML

[S46] C++：函数模板
来源：http://baike.fktsv.cn/Article/details/gnvghjawf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gearcyico.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.vehdjk.com/Article/details/gmwidxjuw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/gwsjuufpp.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gobwxkhjq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gpteqkcwl.sHtML


<!-- 参考信息 -->