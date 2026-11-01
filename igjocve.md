代发 wailian999

ANALYZE TABLE users;
来源：http://3g.vehdjk.com/Article/details/grkgmirqk.sHtML

[Q71] 查看建表语句
来源：http://www.share.sjlbkw.cn/Article/details/gjwrcsdmi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.sjlbkw.cn/Article/details/gscjgthpk.sHtML

[Q72] 查看索引
来源：http://mobile.tarul.cn/Article/details/gvotfwvje.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fktsv.cn/Article/details/grnypqlyi.sHtML

[Q73] 查看表状态
来源：http://mobile.tarul.cn/Article/details/grwvisqwl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gcvhriucg.sHtML

[Q74] 强制使用索引
来源：http://baike.fktsv.cn/Article/details/gznhwuvqm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gvdbunhgn.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gvcpnvzbv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gmndsciea.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.tarul.cn/Article/details/guihorkad.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/gifhlxaux.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.tarul.cn/Article/details/ggpmbcnxm.sHtML

[Q77] 时间加减
来源：http://baike.sjlbkw.cn/Article/details/galgplpts.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gmwyvtsjt.sHtML

[Q78] 当前时间
来源：http://blog.epnwcf.com/Article/details/gcumeopdq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.tarul.cn/Article/details/gtcgrgeso.sHtML

[Q79] 字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/griurnozx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/gcsgmtvbz.sHtML

[Q80] 字符串截取
来源：http://3g.epnwcf.com/Article/details/gqsjzwxml.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.epnwcf.com/Article/details/ghhoyszrx.sHtML

[Q81] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gbgkfndvr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gycehrgrv.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.bbcook.cn/Article/details/gpuiabmdp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gsgudcxsk.sHtML

[Q83] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gdrmoxxvc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gzolodlrp.sHtML

[Q84] 去除首尾空格
来源：http://3g.yfazqb.com/Article/details/grrpjxvws.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gyjrlbmfb.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/ghtcupkxp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/guykwchub.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fktsv.cn/Article/details/gkawaslmq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.yfazqb.com/Article/details/gyfmzljzs.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/gqyertdgt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fktsv.cn/Article/details/gdcsbzfch.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fktsv.cn/Article/details/gjxeylfuf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gueyxjdft.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.yfazqb.com/Article/details/giksgoxqt.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gvusdsopw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsddwbfy.sHtML

[Q90] 生成序号列
来源：http://blog.vehdjk.com/Article/details/gqgdtrqzw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.vehdjk.com/Article/details/gjtvjcrhf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/giocqmanv.sHtML

R. Bash 专题
来源：http://read.share.tarul.cn/Article/details/gfxyglbwm.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjtjaajyc.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/geoqheoje.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/gduldkeuu.sHtML

set -euo pipefail
来源：http://mobile.tarul.cn/Article/details/gafhqakrp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gemboyvrv.sHtML

name="Tom"; echo "$name"
来源：http://mobile.bbcook.cn/Article/details/gukpnjlfh.sHtML

[R03] 只读变量
来源：http://www.share.yfazqb.com/Article/details/goozztyhh.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/goffzuths.sHtML

[R04] 位置参数
来源：http://3g.yfazqb.com/Article/details/gwamzpwve.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.yfazqb.com/Article/details/gszboxueb.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gpssqiguq.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gkqljipks.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/glwfqrsxa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/grtnoshqv.sHtML

[R07] if 判断文件
来源：http://www.m.share.yfazqb.com/Article/details/gwquxqiwv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.yfazqb.com/Article/details/gykvhrheo.sHtML

[R08] 数值比较
来源：http://baike.yfazqb.com/Article/details/gqptieznk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fktsv.cn/Article/details/glgbjtlkp.sHtML

[R09] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/gfaioiuwc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/gwessgmeb.sHtML

[R10] 正则匹配
来源：http://3g.tarul.cn/Article/details/gkeozydnq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/gldqogwgr.sHtML

[R11] case 多分支
来源：http://m.share.vehdjk.com/Article/details/gwepzoyof.sHtML

case "$1" in
来源：http://wap.vehdjk.com/Article/details/gcntekoal.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gptwbzukw.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdsyhyil.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.vehdjk.com/Article/details/gqndqsfiv.sHtML

esac
来源：http://www.blog.vehdjk.com/Article/details/gaeqfmbdv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.tarul.cn/Article/details/grvkbwfpj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fktsv.cn/Article/details/gywyujayl.sHtML

[R13] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gikfttnzn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gsahdeyrg.sHtML

[R14] C 风格 for
来源：http://www.blog.fktsv.cn/Article/details/gspqrlkbf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gxpdyndyh.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gfuwzeewb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.bbcook.cn/Article/details/gqhzqstgn.sHtML

[R16] until 等待条件
来源：http://wap.yfazqb.com/Article/details/gdljygtzd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gkvaykzoy.sHtML

[R17] 数组定义与取值
来源：http://www.blog.yfazqb.com/Article/details/gfrpqatgl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/gkjwqmqms.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gpahgnein.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/gontcmtej.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gwoxvgnrp.sHtML

echo "${#arr[@]}"
来源：http://mobile.fktsv.cn/Article/details/ggodixpll.sHtML

[R20] 关联数组（字典）
来源：http://wap.fktsv.cn/Article/details/gwrvlxnvd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/gfgzyjnmz.sHtML

[R21] 字符串长度
来源：http://www.blog.fktsv.cn/Article/details/guezdgnqi.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/gtndzjjoj.sHtML

[R22] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gnzocvzso.sHtML

echo "${s:0:5}"
来源：http://read.share.sjlbkw.cn/Article/details/gaoyzwtiy.sHtML

[R23] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gjqclrlgs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/gdpkwwdhr.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gcegsweup.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.tarul.cn/Article/details/grbuwfigj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.bbcook.cn/Article/details/glvpwmbtt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.vehdjk.com/Article/details/gptrnmgau.sHtML

[R26] 命令替换
来源：http://mobile.tarul.cn/Article/details/gunenzfdk.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.tarul.cn/Article/details/gtpytmkgi.sHtML

[R27] 算术展开
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqjjgbdw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/grojgewei.sHtML

[R28] 浮点运算
来源：http://www.blog.bbcook.cn/Article/details/guyedlyzg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.sjlbkw.cn/Article/details/gvbaslmyv.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/ggpywjbft.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.bbcook.cn/Article/details/gipcbuavn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.sjlbkw.cn/Article/details/glkrgomce.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/guctvitxg.sHtML

[R31] 局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gselqcksf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.vehdjk.com/Article/details/gpepncnpo.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/gzmseggaf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/gqsnpzovj.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.sjlbkw.cn/Article/details/gszqgsdvb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.epnwcf.com/Article/details/gblofnple.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/glljwtoaw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/giosqpzkw.sHtML

[R35] 后台执行并等待
来源：http://m.share.vehdjk.com/Article/details/gmybrzcvw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gtqmtegff.sHtML

[R36] 并发执行多个任务
来源：http://www.share.yfazqb.com/Article/details/gcdriglcn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.yfazqb.com/Article/details/gubfhpkqc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/gnxmbwpru.sHtML

files=$(ls -1)
来源：http://wap.vehdjk.com/Article/details/gijrmiqhr.sHtML

[R38] 管道串联
来源：http://blog.bbcook.cn/Article/details/gaeoquefo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.yfazqb.com/Article/details/gwiaknaqu.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.yfazqb.com/Article/details/gudkxthlm.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/gzohrrews.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gmdnnwkla.sHtML

echo "log" >> out.log
来源：http://www.m.share.vehdjk.com/Article/details/grrzckekj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gtaasidjq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fktsv.cn/Article/details/gybdrzuer.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gbpsvhenm.sHtML

wc -l < a.txt
来源：http://www.share.epnwcf.com/Article/details/gqtnkuynn.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/gekayprei.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gceapwcpl.sHtML

[R44] 按修改时间查找
来源：http://baike.vehdjk.com/Article/details/gocmxppfd.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gcsnpjpmn.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/gmmdvaibx.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gjuvmoevc.sHtML

[R46] 递归替换文件内容
来源：http://read.share.tarul.cn/Article/details/gbgnfximq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.vehdjk.com/Article/details/gnagqpvfp.sHtML

[R47] sed 单行替换
来源：http://www.m.share.vehdjk.com/Article/details/gzmzqdhhf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gqpbyxkyd.sHtML

[R48] awk 取指定列
来源：http://3g.fktsv.cn/Article/details/geojzpsvh.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gqwiaiofn.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/gxdfxmten.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fktsv.cn/Article/details/guqzpwhqf.sHtML

[R50] awk 求和
来源：http://m.share.bbcook.cn/Article/details/gxlwiodzy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.yfazqb.com/Article/details/ggwtwpyna.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/gtcjiljni.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gpsqavleb.sHtML

[R52] 统计行数
来源：http://blog.fktsv.cn/Article/details/gxjnmrmfd.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/grauaugyb.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.bbcook.cn/Article/details/gdjvfstgj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gjtxjetuo.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/ghaxuiokh.sHtML

diff a.txt b.txt
来源：http://blog.vehdjk.com/Article/details/gobeetsji.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gohtjkefd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gpjteqpwh.sHtML

[R56] 远程拷贝
来源：http://read.share.vehdjk.com/Article/details/ggsnzfqkj.sHtML

scp file user@host:/path/
来源：http://www.blog.tarul.cn/Article/details/gbbkzgzsu.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/gjmbywyvb.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gebdbhcjl.sHtML

[R58] 下载文件
来源：http://3g.vehdjk.com/Article/details/gszfwzobm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.vehdjk.com/Article/details/gbsxcnopw.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gytfpwbhy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/gqfkmyjol.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gjmnsmand.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfmcjavm.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/gnypaoayb.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gprkrhxut.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/gblaooyzi.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/gqiyyazyr.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gxerpfxhf.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fktsv.cn/Article/details/gpiqcvoac.sHtML

[R64] 结束进程
来源：http://wap.sjlbkw.cn/Article/details/gxlbzbaza.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/giyddemll.sHtML

[R65] 查看端口占用
来源：http://wap.tarul.cn/Article/details/gwwgpijha.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/gskhfkduu.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/ghxghyljx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.vehdjk.com/Article/details/gcssbvict.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gmedvvmbq.sHtML

openssl rand -hex 16
来源：http://read.share.yfazqb.com/Article/details/gxyyaflzl.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gwwpidcao.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/gjjfizsaw.sHtML

[R69] 生成随机密码
来源：http://www.share.tarul.cn/Article/details/gbeicwuuw.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.bbcook.cn/Article/details/gymgfqkvh.sHtML

[R70] 时间戳与互转
来源：http://www.blog.epnwcf.com/Article/details/grxrqxouv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/ggrzkjors.sHtML

[R71] 日期格式化
来源：http://blog.epnwcf.com/Article/details/goplbfysp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.tarul.cn/Article/details/gkykwxwms.sHtML

[R72] 等待端口就绪
来源：http://www.blog.tarul.cn/Article/details/gzwjykzxo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/guatdrzhs.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/godijghwx.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/gzmnglffh.sHtML

[R74] 批量重命名
来源：http://m.share.vehdjk.com/Article/details/gexhvqyzj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/grmrphrgn.sHtML

[R75] 导出环境变量
来源：http://read.share.vehdjk.com/Article/details/gvrsmcsaz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fktsv.cn/Article/details/gsfosxlce.sHtML

[R76] 使用临时文件
来源：http://www.share.vehdjk.com/Article/details/gxbyhcint.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gwksozzbc.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/gowwaeskf.sHtML

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/ghcrfsxsr.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/grlrdnepj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.bbcook.cn/Article/details/gyyvptcuv.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gnejykazi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fktsv.cn/Article/details/gdkjtjxxd.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.yfazqb.com/Article/details/gjpjbdyzt.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gbjebhbto.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glmrbjhky.sHtML

S. C / C++ 专题
来源：http://www.blog.epnwcf.com/Article/details/glfzhudgu.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gekuhkcve.sHtML

[S01] C：Hello World
来源：http://www.blog.fktsv.cn/Article/details/govguqthi.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/gvljxkrpt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gjpymmeqn.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gvgdjfxtg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.sjlbkw.cn/Article/details/glphwhkfn.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/ggxemuund.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gtilwawfu.sHtML

[S04] C：字符串复制
来源：http://3g.yfazqb.com/Article/details/gxmnmikzm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.tarul.cn/Article/details/ggckttpkb.sHtML

[S05] C：字符串长度
来源：http://3g.bbcook.cn/Article/details/giawtrzrk.sHtML

strlen(s)
来源：http://read.share.vehdjk.com/Article/details/gekdfqfkk.sHtML

[S06] C：字符串比较
来源：http://blog.epnwcf.com/Article/details/gtfcakrhb.sHtML

strcmp(a, b) == 0
来源：http://read.share.tarul.cn/Article/details/gzqgexjbv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gdbatpgnp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.yfazqb.com/Article/details/gncpbszvy.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/gifxojjtc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.bbcook.cn/Article/details/gauuoyyao.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gagbtcwgp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.yfazqb.com/Article/details/gnsbylzia.sHtML

[S10] C：指针与解引用
来源：http://3g.epnwcf.com/Article/details/ghldlloeo.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/grcphzxwd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gtleipfkg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/gjszltftj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/gcskscpcy.sHtML

fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gzajzsdum.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqcqepae.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/gcizneecc.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/gskmxqvnt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/grkbadjfp.sHtML

[S14] C：枚举
来源：http://3g.epnwcf.com/Article/details/ghpfhsfcy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.epnwcf.com/Article/details/glkpcjahu.sHtML

[S15] C：类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gzpukpczz.sHtML

(double) a / b
来源：http://www.share.tarul.cn/Article/details/gqxwnhowh.sHtML

[S16] C：位操作置位
来源：http://wap.yfazqb.com/Article/details/gdoycfpbc.sHtML

x |= (1 << 3);
来源：http://www.m.share.bbcook.cn/Article/details/gvseuhzlo.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gfqmdaikx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmkmvrpg.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/gpluodein.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gcsubhbuy.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/gwdnfyhvn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gpovgoduf.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/gaqezcyxf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gowzbjexs.sHtML

[S21] C：字符类别判断
来源：http://blog.bbcook.cn/Article/details/gnogtyvdi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/giyifvlcx.sHtML

[S22] C：字符串转数字
来源：http://baike.epnwcf.com/Article/details/giovhotqq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gpqvfwcka.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gnmucxlyc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gfihrqluj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.tarul.cn/Article/details/grjmktjjc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/gctrvpfta.sHtML

[S25] C：内存拷贝
来源：http://m.share.fktsv.cn/Article/details/gdkexzrrp.sHtML

memcpy(dst, src, n);
来源：http://mobile.yfazqb.com/Article/details/ghdalnnsw.sHtML

[S26] C：内存清零
来源：http://wap.yfazqb.com/Article/details/gksytquws.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fktsv.cn/Article/details/gxvuddxda.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/gcsrrmury.sHtML

const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gvlubtkau.sHtML

[S28] C：静态变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gifqnjomh.sHtML

static int counter = 0;
来源：http://www.m.share.tarul.cn/Article/details/grfspmfzq.sHtML

[S29] C：变参函数
来源：http://www.m.share.fktsv.cn/Article/details/ghgzemrby.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gtrqloyzu.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/gnsgezqdp.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gwbmddhts.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/gtgscwiep.sHtML

#endif
来源：http://blog.epnwcf.com/Article/details/gqrraruuv.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gyzirxijo.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/gbfcwxsps.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.bbcook.cn/Article/details/gseiqztzv.sHtML

[S32] C++：字符串
来源：http://baike.yfazqb.com/Article/details/gmsxpqgkx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.epnwcf.com/Article/details/gzxhhdmbd.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/ghljwrhin.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.epnwcf.com/Article/details/grxbklhmg.sHtML

[S34] C++：遍历 vector
来源：http://www.share.yfazqb.com/Article/details/gmqllinyo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/gjiyvipjy.sHtML

[S35] C++：map
来源：http://m.share.bbcook.cn/Article/details/gcssbjhhl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/ggcoqkbud.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gahjminut.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gacebccxn.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gfpnmomsa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/gjbiabmjk.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gbfqklezs.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/gbdjfrgfi.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/gjhkxltzl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.epnwcf.com/Article/details/gncxpwpmn.sHtML

[S40] C++：查找元素
来源：http://blog.tarul.cn/Article/details/gayjcjiti.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.vehdjk.com/Article/details/gcsrddrop.sHtML


<!-- 参考信息 -->