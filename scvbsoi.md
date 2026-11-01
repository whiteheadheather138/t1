代发 wailian999

[Q78] 当前时间
来源：http://www.blog.tarul.cn/Article/details/gwttsrxxc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fktsv.cn/Article/details/gixewnatj.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/gyoulregz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gznqanjws.sHtML

[Q80] 字符串截取
来源：http://read.share.fktsv.cn/Article/details/gmyoziozb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fktsv.cn/Article/details/ggssxozkt.sHtML

[Q81] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gikrobgtb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gkmblblya.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.sjlbkw.cn/Article/details/grdnkrsdc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/ghpfodzed.sHtML

[Q83] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gbkzvbgyx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/glsiwyrpw.sHtML

[Q84] 去除首尾空格
来源：http://mobile.bbcook.cn/Article/details/gewzdfgvo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gizuwyprm.sHtML

[Q85] 数值取整
来源：http://blog.sjlbkw.cn/Article/details/gbatbrpzl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fktsv.cn/Article/details/gftrrpqhf.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gkztvlfwe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.vehdjk.com/Article/details/gqkfcarnh.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.sjlbkw.cn/Article/details/gpbvvetqm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gsgmrgtyx.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/gcdkshoys.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gfawcnfnp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.epnwcf.com/Article/details/gotalzwtp.sHtML

[Q89] 判断表是否存在
来源：http://blog.epnwcf.com/Article/details/gslwimlwi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.epnwcf.com/Article/details/gljysjpmb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.tarul.cn/Article/details/gquopflcg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.tarul.cn/Article/details/gwkinhzic.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gksudmitd.sHtML

R. Bash 专题
来源：http://www.share.vehdjk.com/Article/details/giecpikon.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjbtwuhag.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.bbcook.cn/Article/details/gflphdgmy.sHtML

#!/usr/bin/env bash
来源：http://3g.bbcook.cn/Article/details/gycxwvvkz.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gxhqglboh.sHtML

[R02] 变量赋值与使用
来源：http://www.share.tarul.cn/Article/details/ghilvcvel.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/girkpxmoh.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/gvjpvvzib.sHtML

readonly PI=3.14
来源：http://baike.epnwcf.com/Article/details/gimmoagot.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gnqxdoopw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.sjlbkw.cn/Article/details/gipnwdecx.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/gqaqkbuwz.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/gbyicaiif.sHtML

[R06] 判断命令是否存在
来源：http://blog.tarul.cn/Article/details/gblylchby.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gpwcbjxjj.sHtML

[R07] if 判断文件
来源：http://read.share.epnwcf.com/Article/details/gztiwbsww.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.yfazqb.com/Article/details/gvfnggyma.sHtML

[R08] 数值比较
来源：http://wap.vehdjk.com/Article/details/ggtxwmayg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.tarul.cn/Article/details/gzvlukayv.sHtML

[R09] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/gvrulteqd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/gwvbediht.sHtML

[R10] 正则匹配
来源：http://baike.bbcook.cn/Article/details/gqaurtqna.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkmwlezo.sHtML

[R11] case 多分支
来源：http://www.m.share.yfazqb.com/Article/details/gbqnbsxpn.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/gpqspqojk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gbpzqkkvx.sHtML

stop)  echo "停止" ;;
来源：http://m.share.vehdjk.com/Article/details/gryyciose.sHtML

*)     echo "未知命令" ;;
来源：http://3g.yfazqb.com/Article/details/gcqmehxit.sHtML

esac
来源：http://3g.yfazqb.com/Article/details/gkcwtbymv.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/gewxkhgli.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.bbcook.cn/Article/details/gznqjpnoe.sHtML

[R13] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/gwdbedmud.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gpqjjljdz.sHtML

[R14] C 风格 for
来源：http://m.share.sjlbkw.cn/Article/details/gxdhjqifa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gyxcznqjq.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gxaqjgkcj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/gnpoyozbl.sHtML

[R16] until 等待条件
来源：http://wap.tarul.cn/Article/details/gjkuhdpjr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gtwtydvpa.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gwfleoimp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.sjlbkw.cn/Article/details/gibnqumww.sHtML

[R18] 遍历数组
来源：http://baike.fktsv.cn/Article/details/gsrghiuxj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gfbnfimqa.sHtML

[R19] 数组长度
来源：http://baike.yfazqb.com/Article/details/gthtkwoks.sHtML

echo "${#arr[@]}"
来源：http://read.share.yfazqb.com/Article/details/gdqrxuyjj.sHtML

[R20] 关联数组（字典）
来源：http://3g.bbcook.cn/Article/details/gdpekipoc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.epnwcf.com/Article/details/gngmapgrc.sHtML

[R21] 字符串长度
来源：http://mobile.bbcook.cn/Article/details/gasaqefdv.sHtML

echo "${#s}"
来源：http://baike.sjlbkw.cn/Article/details/gxvcvtpxa.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gscqxukde.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/gmbnytlgx.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gwnupdqgs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/gnwhcsczr.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gslbucorn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fktsv.cn/Article/details/gosfkknix.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/goiujsyrh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fktsv.cn/Article/details/gzonxuzuw.sHtML

[R26] 命令替换
来源：http://m.share.vehdjk.com/Article/details/gecgboxpl.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.yfazqb.com/Article/details/gmlegvclk.sHtML

[R27] 算术展开
来源：http://wap.yfazqb.com/Article/details/gevhfsrmv.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.tarul.cn/Article/details/gpxxuksqb.sHtML

[R28] 浮点运算
来源：http://baike.yfazqb.com/Article/details/gqmgfltpq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.tarul.cn/Article/details/gvhcygigr.sHtML

[R29] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gmanzamie.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/gyavahctv.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gnjcleqla.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/gfwqedubu.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/grvvwqode.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.tarul.cn/Article/details/gxbfiiuno.sHtML

[R32] 参数个数校验
来源：http://mobile.fktsv.cn/Article/details/gkbkufdsa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gckhmfzjr.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.vehdjk.com/Article/details/gregtfxnt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.tarul.cn/Article/details/gzszexvzh.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gfuukroxi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gltnfmswm.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gcsinswgz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.tarul.cn/Article/details/gkfnvodnn.sHtML

[R36] 并发执行多个任务
来源：http://www.share.bbcook.cn/Article/details/ghofiogls.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.vehdjk.com/Article/details/gnoxstdwg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gwongntll.sHtML

files=$(ls -1)
来源：http://baike.sjlbkw.cn/Article/details/gwvudibqi.sHtML

[R38] 管道串联
来源：http://www.share.yfazqb.com/Article/details/gopmzjrmw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.bbcook.cn/Article/details/gftzpwlga.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/gkluwswbv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/gdskboiyi.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gxcqrfyut.sHtML

echo "log" >> out.log
来源：http://read.share.fktsv.cn/Article/details/gibvpmwyz.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/goblyiwxl.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/gldsngkaq.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/ghipaoxyf.sHtML

wc -l < a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gekqrdeta.sHtML

[R43] 按名字查找文件
来源：http://mobile.tarul.cn/Article/details/gtneqnosy.sHtML

find . -name "*.log" -type f
来源：http://mobile.fktsv.cn/Article/details/gtvoppbse.sHtML

[R44] 按修改时间查找
来源：http://www.blog.vehdjk.com/Article/details/gpyopdaqv.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/grmhiwlxg.sHtML

[R45] 批量删除
来源：http://read.share.yfazqb.com/Article/details/gmsqgoqnx.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/gdiehkkxe.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gxuihnqgh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/gskhyplmu.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/ganomboef.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.bbcook.cn/Article/details/gmvnnexwj.sHtML

[R48] awk 取指定列
来源：http://baike.sjlbkw.cn/Article/details/gfjfgxtpy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gunbngqit.sHtML

[R49] awk 带条件
来源：http://www.share.vehdjk.com/Article/details/gilwzmyfp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.epnwcf.com/Article/details/gzekitcjc.sHtML

[R50] awk 求和
来源：http://baike.vehdjk.com/Article/details/guhewejmo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.epnwcf.com/Article/details/guueaglfr.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/ggrteotfb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.vehdjk.com/Article/details/gqjhmodpc.sHtML

[R52] 统计行数
来源：http://www.blog.vehdjk.com/Article/details/ghzgzafei.sHtML

wc -l a.txt
来源：http://baike.tarul.cn/Article/details/gigmbrjgx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.vehdjk.com/Article/details/glahcjcat.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fktsv.cn/Article/details/gdugxluwq.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gsjybpvpz.sHtML

diff a.txt b.txt
来源：http://m.share.fktsv.cn/Article/details/gsudivsri.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/gizqlildo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/gxsdiupxe.sHtML

[R56] 远程拷贝
来源：http://3g.tarul.cn/Article/details/gcvtnweki.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gxlsbleme.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gwfkuggpo.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gromvslem.sHtML

[R58] 下载文件
来源：http://mobile.bbcook.cn/Article/details/ghdvljwde.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/glaasrkwe.sHtML

[R59] 发 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gpadewsla.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.bbcook.cn/Article/details/gzaubkoxq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gjmhbdche.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fktsv.cn/Article/details/gmidotyyz.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gzbqicicz.sHtML

df -h;  du -sh *
来源：http://wap.vehdjk.com/Article/details/gerbgzwmi.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gthfecqbm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/gytjipbga.sHtML

[R63] 内存与进程
来源：http://3g.fktsv.cn/Article/details/gmierozcb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gbgjwloox.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/ghxcxwndh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gevahudvc.sHtML

[R65] 查看端口占用
来源：http://wap.bbcook.cn/Article/details/gktufxkid.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/gohiufkee.sHtML

[R66] 定时任务
来源：http://www.m.share.fktsv.cn/Article/details/gktgeblip.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gyqmmjhzu.sHtML

[R67] 生成随机十六进制串
来源：http://3g.bbcook.cn/Article/details/gmnjminxk.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gxkznepbh.sHtML

[R68] 计算文件校验值
来源：http://m.share.tarul.cn/Article/details/gwxipocyp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gwhsbzbye.sHtML

[R69] 生成随机密码
来源：http://mobile.epnwcf.com/Article/details/gauxbjtgq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gxbcyiasn.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gjwvfsnnc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/gkgkkwktn.sHtML

[R71] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gueuzippr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/gswdquwmj.sHtML

[R72] 等待端口就绪
来源：http://3g.yfazqb.com/Article/details/gdyfjmtdh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/grgabsvsk.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/gfltugkvm.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gumbkcodn.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/gdrqrlzns.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/gdvqrunrk.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/gjxycvqpo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/gaasfqckp.sHtML

[R76] 使用临时文件
来源：http://read.share.epnwcf.com/Article/details/gkyjaoorw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gjqbpdtgg.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/gydhdvnvs.sHtML

read -rp "请输入: " ans
来源：http://3g.vehdjk.com/Article/details/gvaqzqsqx.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gxedjowby.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/glfyzqhsh.sHtML

[R79] 解析命令行选项
来源：http://wap.vehdjk.com/Article/details/gcezpielh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/gbfgoeqic.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/gqqvkmhow.sHtML

time ./run.sh
来源：http://m.share.yfazqb.com/Article/details/gpqdimnrh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmivnclxp.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrlvuxtk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnqkjofbq.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gjvocesod.sHtML

#include <stdio.h>
来源：http://wap.epnwcf.com/Article/details/gxqrldehh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/gfkkeaeea.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/glwlwutyy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/gzicbnuph.sHtML

[S03] C：读入整数
来源：http://3g.bbcook.cn/Article/details/gzgkblqen.sHtML

int x; scanf("%d", &x);
来源：http://wap.sjlbkw.cn/Article/details/gabntrxyn.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/ggzcwyvan.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gcuunctyh.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/gganaxzql.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/gthqmjums.sHtML

[S06] C：字符串比较
来源：http://www.share.bbcook.cn/Article/details/gjfqqufzc.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gvdwbyotn.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/gnffbzfri.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.vehdjk.com/Article/details/gnnnpbegl.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gplrtjbzf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fktsv.cn/Article/details/gvfhrvgwa.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fktsv.cn/Article/details/gpkhwjvxy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.tarul.cn/Article/details/ghumlpecc.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/gavwbatnp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gpqizbpzl.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gihedgzar.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/gsrusabdo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gswchjzup.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gcvciqjfk.sHtML

[S12] C：写文件
来源：http://m.share.yfazqb.com/Article/details/gwxnzlixo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/gastyqgpn.sHtML

[S13] C：宏定义
来源：http://www.blog.yfazqb.com/Article/details/gbqzlvoun.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.vehdjk.com/Article/details/glifhgscl.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gqkayxneo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.tarul.cn/Article/details/gdgnvmtra.sHtML

[S15] C：类型转换
来源：http://wap.tarul.cn/Article/details/giepxjnep.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gcjlpbdjk.sHtML

[S16] C：位操作置位
来源：http://read.share.sjlbkw.cn/Article/details/gyuhmwtiy.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gezzvmxtk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoqrobwe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fktsv.cn/Article/details/gxuuyunce.sHtML

[S18] C：命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gathnedjo.sHtML

int main(int argc, char **argv)
来源：http://wap.fktsv.cn/Article/details/guqhghumy.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/ghbjlfteq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gmoffabjm.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/gswctspaa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gwcnbissv.sHtML

[S21] C：字符类别判断
来源：http://blog.epnwcf.com/Article/details/gyxtzizxx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/gunrqzdov.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gishqwuxs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fktsv.cn/Article/details/gjvwltlpc.sHtML

[S23] C：随机数
来源：http://wap.yfazqb.com/Article/details/gduvdgdbd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/gackdxrmt.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gctsmbhcc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/gmyiymfhf.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fktsv.cn/Article/details/ghtnmcdfa.sHtML

memcpy(dst, src, n);
来源：http://m.share.epnwcf.com/Article/details/gthnlhaha.sHtML

[S26] C：内存清零
来源：http://blog.yfazqb.com/Article/details/gpoejnnmu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/gsiehxfgt.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/gcurkcbjd.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gejqyyznj.sHtML

[S28] C：静态变量
来源：http://mobile.tarul.cn/Article/details/guuyrxksg.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gxaibmfua.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gyeprwsal.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fktsv.cn/Article/details/gxifstjxe.sHtML

[S30] C：头文件保护
来源：http://www.blog.sjlbkw.cn/Article/details/glnacczgi.sHtML

#ifndef X_H
来源：http://www.share.sjlbkw.cn/Article/details/gbdoefien.sHtML

#define X_H
来源：http://m.share.epnwcf.com/Article/details/gjuvpoats.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gynuxhigc.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gpcolpdcs.sHtML

#include <iostream>
来源：http://m.share.yfazqb.com/Article/details/gtaalvcjk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.tarul.cn/Article/details/gbodyijlb.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gzvttdkgi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.bbcook.cn/Article/details/ghfthdvgy.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/gxlhxpmpr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fktsv.cn/Article/details/ghctasrdt.sHtML

[S34] C++：遍历 vector
来源：http://3g.sjlbkw.cn/Article/details/gjvpifdqo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/gxhtduvdp.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/ghezkjyud.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gihauqwbu.sHtML

[S36] C++：unordered_map
来源：http://www.blog.tarul.cn/Article/details/guvnnznop.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gfllokeow.sHtML

[S37] C++：set
来源：http://baike.bbcook.cn/Article/details/gmhtzvvac.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/ggwpysycl.sHtML

[S38] C++：排序
来源：http://www.blog.vehdjk.com/Article/details/gwovzxzsi.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gwegiuzdl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gbrkbrxps.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/gebejbjok.sHtML

[S40] C++：查找元素
来源：http://mobile.fktsv.cn/Article/details/gbvkukmqv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/gcteyewjf.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/giyxskwlp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.bbcook.cn/Article/details/gmsvkmtsz.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gfjryjalp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.sjlbkw.cn/Article/details/grvcawzno.sHtML

[S43] C++：智能指针
来源：http://www.share.vehdjk.com/Article/details/ggpuwquyl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gwqddycxz.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gumvzpobo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.epnwcf.com/Article/details/gveszqspa.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gadusudtw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gywqwpixe.sHtML

[S46] C++：函数模板
来源：http://m.share.yfazqb.com/Article/details/gvgzzbyuz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/gqxtntxjr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gisiwdcxr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.tarul.cn/Article/details/glbepcpve.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/guqualnwo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/gwpjiriic.sHtML


<!-- 参考信息 -->