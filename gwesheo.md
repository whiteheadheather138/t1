代发 wailian999

SHOW INDEX FROM users;
来源：http://3g.yfazqb.com/Article/details/gfdwwecdw.sHtML

[Q73] 查看表状态
来源：http://m.share.fktsv.cn/Article/details/gjeobogjf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/gxxsszeoi.sHtML

[Q74] 强制使用索引
来源：http://read.share.bbcook.cn/Article/details/giyjrcbaq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/geqydytmh.sHtML

[Q75] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gyciktrda.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gufviqeog.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gujnsdlga.sHtML

[Q76] 按天统计
来源：http://mobile.epnwcf.com/Article/details/gptvuczhm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gxdsshuul.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/gcdcwfepp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gpfkijwyz.sHtML

[Q78] 当前时间
来源：http://mobile.sjlbkw.cn/Article/details/grrfdxklk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fktsv.cn/Article/details/gbfwnjftz.sHtML

[Q79] 字符串拼接
来源：http://baike.fktsv.cn/Article/details/gdhparslg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/geniomvxt.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/gdgumvgpv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gorutzodx.sHtML

[Q81] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gqwhkdgxz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gnorelgwn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.yfazqb.com/Article/details/goiigcvtz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gcsigqivj.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/goxwwmkbj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gowoeocaj.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fktsv.cn/Article/details/gexeddqxh.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/grbqepney.sHtML

[Q85] 数值取整
来源：http://wap.sjlbkw.cn/Article/details/gjiwmobsh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/gybuwcfow.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.sjlbkw.cn/Article/details/gykzebsbc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/gnmhepspv.sHtML

[Q87] JSON 字段做条件
来源：http://blog.epnwcf.com/Article/details/gjynkvbue.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.epnwcf.com/Article/details/gereelgxs.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/gvvloppsm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/gvjxioqbj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/ghfqkpepk.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/gdwihwmqc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.bbcook.cn/Article/details/gubdwxogn.sHtML

[Q90] 生成序号列
来源：http://www.share.tarul.cn/Article/details/gawtrvyto.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.bbcook.cn/Article/details/ggdcofnps.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfxxlwqsd.sHtML

R. Bash 专题
来源：http://www.blog.bbcook.cn/Article/details/gtqjcxvrs.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmpshendt.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/gupqfonev.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gtmrwsfxe.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/griyzmsbz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.sjlbkw.cn/Article/details/gsimsehhp.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/ghgrertbp.sHtML

[R03] 只读变量
来源：http://3g.tarul.cn/Article/details/gidmxconj.sHtML

readonly PI=3.14
来源：http://baike.yfazqb.com/Article/details/ggottgmbf.sHtML

[R04] 位置参数
来源：http://mobile.fktsv.cn/Article/details/ghpyamoic.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.bbcook.cn/Article/details/gnwhxokca.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/gcwuqiena.sHtML

name="${1:-default}"
来源：http://read.share.sjlbkw.cn/Article/details/gclgfazna.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gvokbglzq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gomxcnduf.sHtML

[R07] if 判断文件
来源：http://mobile.bbcook.cn/Article/details/gfaeowrha.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.bbcook.cn/Article/details/gbolfesbo.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/gacdubcxt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gwikegbon.sHtML

[R09] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/ghywfehui.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.epnwcf.com/Article/details/gwmhkilid.sHtML

[R10] 正则匹配
来源：http://www.blog.tarul.cn/Article/details/gaeibfkfb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.bbcook.cn/Article/details/gbauhpmbt.sHtML

[R11] case 多分支
来源：http://3g.tarul.cn/Article/details/gmgxvygob.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gqcxvlqjf.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/goosnjkaw.sHtML

stop)  echo "停止" ;;
来源：http://m.share.bbcook.cn/Article/details/gdoufxhga.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/gqclisney.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/gynbljash.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/gysizxjoc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.bbcook.cn/Article/details/gigsoanfp.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gigyxgvyb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/guyxoiqbm.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/gtfohakhg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gbtfzcueb.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/gfnxmontz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fktsv.cn/Article/details/gwslcmiuq.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gbdyrqafa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gzavzmvew.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.epnwcf.com/Article/details/gwnpktzpx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/gfoighlbt.sHtML

[R18] 遍历数组
来源：http://3g.bbcook.cn/Article/details/gdaxgcauu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/gizgmksex.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/ggcrhbpqf.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gbkvsemvd.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gsowblmsv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.yfazqb.com/Article/details/gfakebmcu.sHtML

[R21] 字符串长度
来源：http://wap.bbcook.cn/Article/details/gsdygssjf.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gyddrrnoe.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkaxfczq.sHtML

echo "${s:0:5}"
来源：http://www.share.fktsv.cn/Article/details/grgzndsqi.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/geqehgvww.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.epnwcf.com/Article/details/gdbipkyjo.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/grbasrprn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gezvxyzsx.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/gcdpufwdj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gqtlvisxn.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/gndojiljn.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.bbcook.cn/Article/details/givcvlics.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gvwcqajgc.sHtML

echo $((1 + 2 * 3))
来源：http://blog.vehdjk.com/Article/details/gyayjnzjc.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gykaeljwf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fktsv.cn/Article/details/gdudgzrqg.sHtML

[R29] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/ggyjifpws.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.tarul.cn/Article/details/gbbwsnpzc.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/gnpfzwovb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.bbcook.cn/Article/details/gpaicysxz.sHtML

[R31] 局部变量
来源：http://www.m.share.vehdjk.com/Article/details/geaupxezr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.epnwcf.com/Article/details/gaqeewrqj.sHtML

[R32] 参数个数校验
来源：http://read.share.epnwcf.com/Article/details/gnrgomrdf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gjptcujfo.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fktsv.cn/Article/details/gazlhwwdi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.vehdjk.com/Article/details/gnyqmvkrg.sHtML

[R34] 退出时清理
来源：http://m.share.bbcook.cn/Article/details/gzmsxtbxl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/geufzcuim.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gttoznayt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/gkfawibrz.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gcpaektxu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.vehdjk.com/Article/details/gabbmifza.sHtML

[R37] 把输出赋给变量
来源：http://mobile.sjlbkw.cn/Article/details/glvtpmlrc.sHtML

files=$(ls -1)
来源：http://read.share.sjlbkw.cn/Article/details/gjoywefef.sHtML

[R38] 管道串联
来源：http://read.share.vehdjk.com/Article/details/gkzmrbcxf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.vehdjk.com/Article/details/garbblihn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/guejbnllo.sHtML

cmd > out.log 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/gluuxiqor.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/gyouafyjd.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/gbrmocgdn.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/gfmjnaebx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.vehdjk.com/Article/details/gxeobbnus.sHtML

[R42] 输入重定向
来源：http://3g.vehdjk.com/Article/details/gqcozywnz.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/gmehvsgtv.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/gkwsxnegr.sHtML

find . -name "*.log" -type f
来源：http://read.share.fktsv.cn/Article/details/gosvukdao.sHtML

[R44] 按修改时间查找
来源：http://blog.yfazqb.com/Article/details/ggcbiezkj.sHtML

find . -mtime -7 -type f
来源：http://wap.tarul.cn/Article/details/gsdxnjzxd.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/gmjhwjuvy.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/gcpgynucf.sHtML

[R46] 递归替换文件内容
来源：http://blog.epnwcf.com/Article/details/gmhktezqm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.yfazqb.com/Article/details/gusxztoua.sHtML

[R47] sed 单行替换
来源：http://baike.vehdjk.com/Article/details/gghcvyrvw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.yfazqb.com/Article/details/gyuosenbm.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gxmhfzbfx.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fktsv.cn/Article/details/gkyjponta.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gevmxprcb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/gdbzhhgbg.sHtML

[R50] awk 求和
来源：http://read.share.bbcook.cn/Article/details/gsovlvthl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/gjxvbvnlu.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/gpmjgamdk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.tarul.cn/Article/details/grlpyxyct.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/gplwuwycy.sHtML

wc -l a.txt
来源：http://baike.vehdjk.com/Article/details/gkhhiiktv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.vehdjk.com/Article/details/gjagbbxlw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/ganjbvmyw.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gueediyec.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/gjdrbqltc.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gdhtjcipy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.epnwcf.com/Article/details/goxgaswxg.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gzhjjbhkj.sHtML

scp file user@host:/path/
来源：http://www.m.share.epnwcf.com/Article/details/griltapfa.sHtML

[R57] 远程执行命令
来源：http://wap.epnwcf.com/Article/details/geaqrnimf.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/gquudegvg.sHtML

[R58] 下载文件
来源：http://baike.epnwcf.com/Article/details/gphxlciqr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.vehdjk.com/Article/details/gdiioroaz.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gvmwwpkkk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.vehdjk.com/Article/details/ggzzzelrp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gyhxssmhb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/gfhsqcmpt.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/gyskrcbrd.sHtML

df -h;  du -sh *
来源：http://baike.vehdjk.com/Article/details/gkvpveuqf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/gvbfsdvks.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.yfazqb.com/Article/details/glajofsbe.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwknykyo.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.epnwcf.com/Article/details/gkxrufqyv.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/gzmgjealg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gyxoebuwv.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/gjemadfyo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/ghwzbudou.sHtML

[R66] 定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gotzfcwwe.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gerkemrkj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/gvqcltewg.sHtML

openssl rand -hex 16
来源：http://3g.tarul.cn/Article/details/gjmhdjkro.sHtML

[R68] 计算文件校验值
来源：http://baike.bbcook.cn/Article/details/gpmuwafwj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.yfazqb.com/Article/details/geccsdvdb.sHtML

[R69] 生成随机密码
来源：http://www.blog.tarul.cn/Article/details/gllooqcih.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fktsv.cn/Article/details/gyrhyrgae.sHtML

[R70] 时间戳与互转
来源：http://mobile.sjlbkw.cn/Article/details/gjhlixxyb.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fktsv.cn/Article/details/gavzaqexe.sHtML

[R71] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gyhtsmmhx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fktsv.cn/Article/details/gsvghchzp.sHtML

[R72] 等待端口就绪
来源：http://mobile.yfazqb.com/Article/details/gquspgdwl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gnvqjxgac.sHtML

[R73] 分割大日志
来源：http://baike.bbcook.cn/Article/details/gulsfvvtj.sHtML

split -l 1000 big.log part_
来源：http://3g.vehdjk.com/Article/details/gdhfkrrxw.sHtML

[R74] 批量重命名
来源：http://baike.sjlbkw.cn/Article/details/gizinfzfa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fktsv.cn/Article/details/gmuxczkgy.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/gzdpkphdt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.yfazqb.com/Article/details/gziptqtiw.sHtML

[R76] 使用临时文件
来源：http://3g.vehdjk.com/Article/details/gkexspkkl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gkverpuxn.sHtML

[R77] 读取用户输入
来源：http://www.share.fktsv.cn/Article/details/gautcueol.sHtML

read -rp "请输入: " ans
来源：http://3g.epnwcf.com/Article/details/gtuaiderm.sHtML

[R78] 交互式菜单
来源：http://3g.vehdjk.com/Article/details/gjebvxsmo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gycweddgx.sHtML

[R79] 解析命令行选项
来源：http://read.share.bbcook.cn/Article/details/gprebmfmj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/gomkgtbkx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.tarul.cn/Article/details/gsizhfmqr.sHtML

time ./run.sh
来源：http://www.m.share.epnwcf.com/Article/details/ghwcpndwf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ghnxfqfca.sHtML

S. C / C++ 专题
来源：http://www.m.share.vehdjk.com/Article/details/gwcbpdupa.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gilprfuwx.sHtML

[S01] C：Hello World
来源：http://read.share.yfazqb.com/Article/details/gohoaetgf.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/gkttxjcyp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gmtiiwfgu.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gysbklbka.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/gocbcscst.sHtML

[S03] C：读入整数
来源：http://baike.fktsv.cn/Article/details/giogknfbn.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gdjlxvgce.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/gxointrtx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gbkigjtuh.sHtML

[S05] C：字符串长度
来源：http://read.share.bbcook.cn/Article/details/gvjajqeec.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gcoscxylr.sHtML

[S06] C：字符串比较
来源：http://3g.bbcook.cn/Article/details/gydebuvxg.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gqiagiqxm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fktsv.cn/Article/details/gtrbztvdw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/gbzqpodrb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.tarul.cn/Article/details/gupjnatwz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/gzfpsxpgf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/ggzmvvvde.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gvgqwypsw.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/gvqyfkqyl.sHtML

int *p = &a;  *p = 5;
来源：http://baike.epnwcf.com/Article/details/gjbspudko.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gzevidtek.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.yfazqb.com/Article/details/gimufzjdh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.epnwcf.com/Article/details/gkdkirrrv.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gupdhgcat.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/gdbhlfmmn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gepksnskm.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/gxkzgtsbp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gssjfipfz.sHtML

[S14] C：枚举
来源：http://blog.sjlbkw.cn/Article/details/gumcethhk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/gsocygxfi.sHtML

[S15] C：类型转换
来源：http://m.share.fktsv.cn/Article/details/gzeaepdab.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxtptzyq.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gkvdbhxiv.sHtML

x |= (1 << 3);
来源：http://3g.yfazqb.com/Article/details/gbklobxnu.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gkcrmzqyg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gmlcgydht.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/gymloyuur.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.epnwcf.com/Article/details/glppzawsg.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gtsldblzq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gwreqqfij.sHtML

[S20] C：二分查找
来源：http://3g.yfazqb.com/Article/details/glfadzbcm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gxornzcbd.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gmcfaghih.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gzoxoeaze.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gqgylvzln.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/grdqlrmtt.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/gvugeayzb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/gjuazesyd.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/giactuduj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/ggvexzfil.sHtML

[S25] C：内存拷贝
来源：http://m.share.epnwcf.com/Article/details/gfyennheq.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/gblncfjma.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gqmejalwq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.sjlbkw.cn/Article/details/gycfxbxcf.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/gisejtxxs.sHtML

const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gpzveolwn.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/gexfperzv.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gzhixmfiz.sHtML

[S29] C：变参函数
来源：http://m.share.epnwcf.com/Article/details/gvfvwtnty.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/gohadgdln.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/grlmqasoj.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gnhkrtmrv.sHtML

#define X_H
来源：http://www.share.vehdjk.com/Article/details/grprgytai.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gactwhddi.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/gwmkzqeft.sHtML

#include <iostream>
来源：http://www.blog.epnwcf.com/Article/details/gmvyphnuo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/guwttjfit.sHtML

[S32] C++：字符串
来源：http://www.blog.yfazqb.com/Article/details/gyizcohnb.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.sjlbkw.cn/Article/details/gzwzlsdsk.sHtML

[S33] C++：vector 增删
来源：http://www.blog.epnwcf.com/Article/details/ghvkjhjok.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gpqxwkiba.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/ghvgmdmdb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.epnwcf.com/Article/details/goxybsbrg.sHtML

[S35] C++：map
来源：http://wap.epnwcf.com/Article/details/ghrrpjyjn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/ggfmdaccp.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/giywxbauy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gwzdfnbar.sHtML

[S37] C++：set
来源：http://www.share.fktsv.cn/Article/details/gexgbyvau.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/gdvliookc.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/gdrhpdvpj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.vehdjk.com/Article/details/gxzwuittx.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gstxajaga.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/grubhoneo.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/gosuaekal.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.sjlbkw.cn/Article/details/gyffywpfx.sHtML

[S41] C++：类与构造函数
来源：http://blog.vehdjk.com/Article/details/gziuqhxuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/gbjkvpjcp.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fktsv.cn/Article/details/gdfueysfy.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/gmfzcigik.sHtML


<!-- 参考信息 -->