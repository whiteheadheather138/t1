代发 wailian999

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/gvepfuwaj.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/ggvdcrxdb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.yfazqb.com/Article/details/gzhupoxui.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gjcujtahx.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/gfmmudtck.sHtML

[Q71] 查看建表语句
来源：http://www.share.bbcook.cn/Article/details/gqrsrakzu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fktsv.cn/Article/details/gndcrajwi.sHtML

[Q72] 查看索引
来源：http://www.share.epnwcf.com/Article/details/gifvpegqj.sHtML

SHOW INDEX FROM users;
来源：http://wap.fktsv.cn/Article/details/gwjbuenig.sHtML

[Q73] 查看表状态
来源：http://www.blog.fktsv.cn/Article/details/gcedicxye.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/ganoaesty.sHtML

[Q74] 强制使用索引
来源：http://www.share.fktsv.cn/Article/details/gcgdncoby.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gknizqfnk.sHtML

[Q75] 日期格式化
来源：http://read.share.tarul.cn/Article/details/ghvtjumzu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gogunhswd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.epnwcf.com/Article/details/gzzoglqgi.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/gwtiuzhvg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/gqdcayant.sHtML

[Q77] 时间加减
来源：http://www.blog.yfazqb.com/Article/details/gqmtadazd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.sjlbkw.cn/Article/details/gcvjssdan.sHtML

[Q78] 当前时间
来源：http://wap.yfazqb.com/Article/details/gllvoouvb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gayrmalip.sHtML

[Q79] 字符串拼接
来源：http://blog.epnwcf.com/Article/details/gdcbaygob.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fktsv.cn/Article/details/gmoazqbur.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/gfhyghewo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/glwjvojnm.sHtML

[Q81] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/giofqzqis.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gedmowfym.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/gkfuurycs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gjsuxnsch.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gvcfmrbpt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gqrolrzbw.sHtML

[Q84] 去除首尾空格
来源：http://3g.yfazqb.com/Article/details/gpfvogbfq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gwmjoovvt.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/gabvmnlzo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.bbcook.cn/Article/details/gezifqpfc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.tarul.cn/Article/details/gakjadgjz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fktsv.cn/Article/details/gnjzdkoft.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.bbcook.cn/Article/details/grrtwoxzk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/gonigmpqu.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.sjlbkw.cn/Article/details/gzxeatjdb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.sjlbkw.cn/Article/details/gwjvwnvzk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gdnhwpslk.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/gkmpxajbp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gvryrcodi.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gqmsyjhnz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/gqvbpfyut.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfprjisfn.sHtML

R. Bash 专题
来源：http://3g.yfazqb.com/Article/details/gypsezuen.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvswiabvk.sHtML

[R01] shebang 与严格模式
来源：http://wap.yfazqb.com/Article/details/gnktahqwq.sHtML

#!/usr/bin/env bash
来源：http://m.share.vehdjk.com/Article/details/gntgalxgs.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/gxmakwvok.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.vehdjk.com/Article/details/gpsvstrjo.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/gwiqtkkls.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gkkuvrdrj.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gfyehpwpx.sHtML

[R04] 位置参数
来源：http://blog.sjlbkw.cn/Article/details/goimbkyet.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.vehdjk.com/Article/details/grypgrnlf.sHtML

[R05] 参数默认值
来源：http://3g.epnwcf.com/Article/details/gahqbnlsm.sHtML

name="${1:-default}"
来源：http://read.share.fktsv.cn/Article/details/gjwkthcke.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/gcbljrtry.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gcfifixki.sHtML

[R07] if 判断文件
来源：http://read.share.bbcook.cn/Article/details/gnteljboo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.bbcook.cn/Article/details/gphopxzmv.sHtML

[R08] 数值比较
来源：http://3g.epnwcf.com/Article/details/gwsommgaq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.epnwcf.com/Article/details/gpaykqocb.sHtML

[R09] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gcdnekpav.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gjvukelui.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/gihdsrbqq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/garchmcwa.sHtML

[R11] case 多分支
来源：http://www.blog.yfazqb.com/Article/details/gaipkjdan.sHtML

case "$1" in
来源：http://baike.yfazqb.com/Article/details/gepgbvuks.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gqgpgyygd.sHtML

stop)  echo "停止" ;;
来源：http://baike.yfazqb.com/Article/details/gpgisahgb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/gwzsvdvaa.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/grtbfkeny.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/gadzekqbd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/gyeiwrfmu.sHtML

[R13] for 计数循环
来源：http://wap.vehdjk.com/Article/details/glrdmsvhd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gvemyviqy.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/ghtibghxo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gewpwwslo.sHtML

[R15] while 逐行读文件
来源：http://blog.yfazqb.com/Article/details/ggfuvhkmq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/gwfjuodyn.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/gttnbikyp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gwnjvwoue.sHtML

[R17] 数组定义与取值
来源：http://mobile.bbcook.cn/Article/details/gmracebns.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/gsaepdtyu.sHtML

[R18] 遍历数组
来源：http://baike.tarul.cn/Article/details/gocouwgri.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.tarul.cn/Article/details/gtaudcdcs.sHtML

[R19] 数组长度
来源：http://blog.bbcook.cn/Article/details/gvgemvtll.sHtML

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/ghysjnohf.sHtML

[R20] 关联数组（字典）
来源：http://baike.epnwcf.com/Article/details/gciagwbyh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.vehdjk.com/Article/details/gnksfprhu.sHtML

[R21] 字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gubrehcul.sHtML

echo "${#s}"
来源：http://read.share.bbcook.cn/Article/details/gprsfjqyd.sHtML

[R22] 截取子串
来源：http://m.share.fktsv.cn/Article/details/gdjompegu.sHtML

echo "${s:0:5}"
来源：http://baike.vehdjk.com/Article/details/glqtlzzbd.sHtML

[R23] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gvdrtlprx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.epnwcf.com/Article/details/gnogqrydb.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/glyjnvmqu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gyndbxksp.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gbfhzviox.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.epnwcf.com/Article/details/gepninmri.sHtML

[R26] 命令替换
来源：http://www.share.epnwcf.com/Article/details/gctzwcjvg.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fktsv.cn/Article/details/gavxqolhk.sHtML

[R27] 算术展开
来源：http://baike.epnwcf.com/Article/details/giezrovpn.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gmhbqvgrn.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gvzyfcbrc.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/gsrlijwzb.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/glaavzvca.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gcukluyyf.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gmauvgtea.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fktsv.cn/Article/details/ggduoteqk.sHtML

[R31] 局部变量
来源：http://www.share.bbcook.cn/Article/details/gjcvifgzq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.sjlbkw.cn/Article/details/ggbkdyrzm.sHtML

[R32] 参数个数校验
来源：http://m.share.bbcook.cn/Article/details/guzyvaxga.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gtpjelfvu.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.sjlbkw.cn/Article/details/gziobrejz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/gmrprosdm.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/gxojyimij.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gkyvkwgku.sHtML

[R35] 后台执行并等待
来源：http://baike.fktsv.cn/Article/details/gopubkqka.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.sjlbkw.cn/Article/details/gvydgvoir.sHtML

[R36] 并发执行多个任务
来源：http://m.share.tarul.cn/Article/details/gbvioaodf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/gzowtlohx.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/geuzxjnxr.sHtML

files=$(ls -1)
来源：http://mobile.bbcook.cn/Article/details/gyulodrrp.sHtML

[R38] 管道串联
来源：http://blog.epnwcf.com/Article/details/gkvojgylj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.vehdjk.com/Article/details/gawpqizff.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/gffqzcuse.sHtML

cmd > out.log 2>&1
来源：http://3g.yfazqb.com/Article/details/greiqnegg.sHtML

[R40] 追加写日志
来源：http://www.blog.epnwcf.com/Article/details/gujhliked.sHtML

echo "log" >> out.log
来源：http://3g.yfazqb.com/Article/details/gagybqvbv.sHtML

[R41] 丢弃输出
来源：http://www.blog.yfazqb.com/Article/details/ghltcsqou.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fktsv.cn/Article/details/gqpqvirut.sHtML

[R42] 输入重定向
来源：http://m.share.yfazqb.com/Article/details/gbkbdjmhv.sHtML

wc -l < a.txt
来源：http://3g.epnwcf.com/Article/details/gkahuwqie.sHtML

[R43] 按名字查找文件
来源：http://3g.bbcook.cn/Article/details/greaorpqe.sHtML

find . -name "*.log" -type f
来源：http://blog.vehdjk.com/Article/details/gziztjtkr.sHtML

[R44] 按修改时间查找
来源：http://wap.sjlbkw.cn/Article/details/grwvugjgo.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/gkixhlsqa.sHtML

[R45] 批量删除
来源：http://3g.epnwcf.com/Article/details/gvbvmyqzh.sHtML

find . -name "*.tmp" -delete
来源：http://blog.bbcook.cn/Article/details/ghrwzokzv.sHtML

[R46] 递归替换文件内容
来源：http://m.share.yfazqb.com/Article/details/gpamtbqfg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.bbcook.cn/Article/details/gohzyrpla.sHtML

[R47] sed 单行替换
来源：http://read.share.vehdjk.com/Article/details/gkklndcth.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gxuixpbzy.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gsammgzuh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gvztzrmtw.sHtML

[R49] awk 带条件
来源：http://3g.bbcook.cn/Article/details/grbwyhpml.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/ghnagxavc.sHtML

[R50] awk 求和
来源：http://read.share.vehdjk.com/Article/details/gvouszsyz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gqzrhfqag.sHtML

[R51] 排序去重取前几
来源：http://wap.vehdjk.com/Article/details/gqbpobuyg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.epnwcf.com/Article/details/gvtsgnftd.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/gohhnnddd.sHtML

wc -l a.txt
来源：http://www.share.sjlbkw.cn/Article/details/ggwyczgnq.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/gzsbplxcb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.sjlbkw.cn/Article/details/gwjxndwrr.sHtML

[R54] 比较两个文件
来源：http://blog.tarul.cn/Article/details/guokupkdu.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/ghxmydjfv.sHtML

[R55] 压缩与解压
来源：http://3g.tarul.cn/Article/details/gumlzjkpa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.epnwcf.com/Article/details/gwmpvfiaj.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/gxrefetfx.sHtML

scp file user@host:/path/
来源：http://m.share.bbcook.cn/Article/details/geozgymhd.sHtML

[R57] 远程执行命令
来源：http://mobile.tarul.cn/Article/details/ganwcsoec.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gffwfnwde.sHtML

[R58] 下载文件
来源：http://wap.yfazqb.com/Article/details/ggpjktixg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fktsv.cn/Article/details/gvosjutdz.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/gjdjlxaqd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.bbcook.cn/Article/details/gurwbqbsd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/goibpshaq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/gjsgbgcnx.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/gbijofjqe.sHtML

df -h;  du -sh *
来源：http://www.share.yfazqb.com/Article/details/gdpbxhghu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/gdixudlvo.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gywgpgswc.sHtML

[R63] 内存与进程
来源：http://3g.yfazqb.com/Article/details/goooeryyg.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gklfjujft.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/gruuevjdk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fktsv.cn/Article/details/grtvmqwoi.sHtML

[R65] 查看端口占用
来源：http://3g.vehdjk.com/Article/details/ghogvqkzi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.bbcook.cn/Article/details/gsxzanrzo.sHtML

[R66] 定时任务
来源：http://m.share.tarul.cn/Article/details/gqrogtkeo.sHtML

crontab -e;  crontab -l
来源：http://m.share.fktsv.cn/Article/details/gwsydqofn.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.tarul.cn/Article/details/gcyuxhmlu.sHtML

openssl rand -hex 16
来源：http://www.blog.sjlbkw.cn/Article/details/glwpodfel.sHtML

[R68] 计算文件校验值
来源：http://blog.sjlbkw.cn/Article/details/gmhbspfqq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/guiahlyor.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/grvjhlnbv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/gvskucysw.sHtML

[R70] 时间戳与互转
来源：http://m.share.epnwcf.com/Article/details/gfhbdxdqy.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.epnwcf.com/Article/details/gdzvdfula.sHtML

[R71] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gfscoflma.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.epnwcf.com/Article/details/gnbnfbjmr.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.epnwcf.com/Article/details/gfsgsfmob.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gtgnzykvb.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/ghrcvhgjy.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/gstjiraat.sHtML

[R74] 批量重命名
来源：http://m.share.vehdjk.com/Article/details/ggpjplblu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/grhuiccja.sHtML

[R75] 导出环境变量
来源：http://www.blog.fktsv.cn/Article/details/gxpzztqwr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fktsv.cn/Article/details/gfjdyridx.sHtML

[R76] 使用临时文件
来源：http://wap.sjlbkw.cn/Article/details/gaiifagxj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gyrpwfwvp.sHtML

[R77] 读取用户输入
来源：http://3g.vehdjk.com/Article/details/ghtuyypwg.sHtML

read -rp "请输入: " ans
来源：http://read.share.sjlbkw.cn/Article/details/gatfildrr.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/glfeevpce.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.bbcook.cn/Article/details/gtzqpqwso.sHtML

[R79] 解析命令行选项
来源：http://mobile.yfazqb.com/Article/details/ghjegjukm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gidseaqlq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.tarul.cn/Article/details/gfitmuspi.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gjigigbty.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gsaucgnsv.sHtML

S. C / C++ 专题
来源：http://wap.sjlbkw.cn/Article/details/ggpvoyzpy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grgufpqoc.sHtML

[S01] C：Hello World
来源：http://read.share.yfazqb.com/Article/details/gbdbphlie.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkvwrmny.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fktsv.cn/Article/details/gufdnpfkh.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.yfazqb.com/Article/details/gafksktdw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/ggnhmpgon.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/gfekehqhp.sHtML

int x; scanf("%d", &x);
来源：http://blog.fktsv.cn/Article/details/glkyvfdok.sHtML

[S04] C：字符串复制
来源：http://m.share.yfazqb.com/Article/details/gefzikhhz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gatbtsepo.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gmewdpvvz.sHtML

strlen(s)
来源：http://www.blog.vehdjk.com/Article/details/gwqkvydyq.sHtML

[S06] C：字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/glexltsut.sHtML

strcmp(a, b) == 0
来源：http://blog.fktsv.cn/Article/details/gjbnrceas.sHtML

[S07] C：数组遍历求和
来源：http://baike.fktsv.cn/Article/details/gvjakdleb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.tarul.cn/Article/details/gnnsctfzn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gnlllfhpk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fktsv.cn/Article/details/grirgggeq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/gjcsyaogx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gsnbjtciv.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/gpgnhahxb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.yfazqb.com/Article/details/gmakpmlnf.sHtML

[S11] C：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gslfrdpkl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fktsv.cn/Article/details/glvksapcw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fktsv.cn/Article/details/gfcsxxrwc.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gewnqidqf.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/gaelbjqow.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.tarul.cn/Article/details/gvaujlayi.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gzalvuplz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gpnjidnzu.sHtML

[S14] C：枚举
来源：http://read.share.sjlbkw.cn/Article/details/gzrnqzchu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/gbgfvblmz.sHtML

[S15] C：类型转换
来源：http://read.share.vehdjk.com/Article/details/gbkqrijqp.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gzttjaulb.sHtML

[S16] C：位操作置位
来源：http://wap.fktsv.cn/Article/details/gdqcszzpt.sHtML

x |= (1 << 3);
来源：http://www.share.tarul.cn/Article/details/gcllrgwxk.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fktsv.cn/Article/details/gdeajizvx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/gzxgackwe.sHtML

[S18] C：命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gvrsdxgkr.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/gxurlhhgn.sHtML

[S19] C：快速排序
来源：http://blog.sjlbkw.cn/Article/details/gnjyiqxok.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gkmvidhad.sHtML

[S20] C：二分查找
来源：http://www.m.share.vehdjk.com/Article/details/gsmvazgoz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gqdmeqlbp.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/geyqjgnah.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.tarul.cn/Article/details/golpwrxbh.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gaqyvhril.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gnfqgzmbf.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/geiljxweh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/gwaxpnssf.sHtML

[S24] C：获取本地时间
来源：http://read.share.epnwcf.com/Article/details/ggsiklaaw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/gmbgawqbt.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gvaoutdym.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gunrbnwty.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/grvodjehb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/ggdavpzte.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/gatjeyjpy.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/ggfutcwlg.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gdvrncvmc.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/goznkwtuj.sHtML

[S29] C：变参函数
来源：http://baike.bbcook.cn/Article/details/gsehvtzdd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.yfazqb.com/Article/details/gvntgvogb.sHtML

[S30] C：头文件保护
来源：http://www.blog.vehdjk.com/Article/details/gbteohjyg.sHtML

#ifndef X_H
来源：http://blog.epnwcf.com/Article/details/gohhurzkq.sHtML

#define X_H
来源：http://mobile.tarul.cn/Article/details/gmwtvrrdi.sHtML

#endif
来源：http://wap.tarul.cn/Article/details/gbgbightf.sHtML

[S31] C++：Hello World
来源：http://baike.bbcook.cn/Article/details/gwsqmrsvs.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/gybfxziqm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/gbitqubia.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/gcsuvlxiv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.vehdjk.com/Article/details/ghaleghkl.sHtML

[S33] C++：vector 增删
来源：http://www.share.tarul.cn/Article/details/gybsupzqq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.vehdjk.com/Article/details/gxgjzosry.sHtML

[S34] C++：遍历 vector
来源：http://3g.bbcook.cn/Article/details/gtcxhpldw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gkhcqbcwo.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/guusjkcej.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gtudnomsd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/gzihsqluv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gwqqbhskb.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/gqvkvxibb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gapfhwyqm.sHtML

[S38] C++：排序
来源：http://www.m.share.tarul.cn/Article/details/gzmvdtwuh.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fktsv.cn/Article/details/gzozvucun.sHtML


<!-- 参考信息 -->