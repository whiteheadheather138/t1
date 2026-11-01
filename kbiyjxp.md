代发 wailian999

ANALYZE TABLE users;
来源：http://mobile.sjlbkw.cn/Article/details/gngamaeuu.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gbknvagwx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.yfazqb.com/Article/details/gktfeqrok.sHtML

[Q72] 查看索引
来源：http://www.share.epnwcf.com/Article/details/grctsqxqm.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gumnwjwov.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gmyyndggh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/gusfqlqry.sHtML

[Q74] 强制使用索引
来源：http://3g.tarul.cn/Article/details/gbmuzcxjj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.vehdjk.com/Article/details/goidlnkdi.sHtML

[Q75] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gpbelhpod.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.bbcook.cn/Article/details/gpuwdugba.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.epnwcf.com/Article/details/gvsdtjgmw.sHtML

[Q76] 按天统计
来源：http://wap.sjlbkw.cn/Article/details/gqbemnanb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.vehdjk.com/Article/details/gagzwydxi.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gejhthiop.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.tarul.cn/Article/details/gskyodazp.sHtML

[Q78] 当前时间
来源：http://3g.epnwcf.com/Article/details/gxrqsylif.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.sjlbkw.cn/Article/details/gxsljgebu.sHtML

[Q79] 字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gwopexrlq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.yfazqb.com/Article/details/gyefdnsqa.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/gkqtextsb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gptapljov.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gsgsgaijt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/golicqwbz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.yfazqb.com/Article/details/gatasdnli.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gvtmxstpr.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gfpfmcodc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gcwxdjjfr.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/gmbfqyjif.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/ggfosknzn.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/ggjpkirwd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/ghfteajsu.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/gtsnsxzcz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gkphjjstb.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gibnelggj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.vehdjk.com/Article/details/gkevbbnsy.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.sjlbkw.cn/Article/details/gisckglrl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.bbcook.cn/Article/details/ggbqkggtz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/gyhilabnq.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/gbnndfafm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.yfazqb.com/Article/details/gtajffuki.sHtML

[Q90] 生成序号列
来源：http://baike.fktsv.cn/Article/details/gimdvxizn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/grrwrsoto.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ganholkqv.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/gmxlnisjl.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmjqibnxg.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/gpemlpdrk.sHtML

#!/usr/bin/env bash
来源：http://m.share.yfazqb.com/Article/details/guiazlpyb.sHtML

set -euo pipefail
来源：http://www.blog.bbcook.cn/Article/details/gzasjdzjd.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gxuwcjayh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gfxyaxniv.sHtML

[R03] 只读变量
来源：http://wap.epnwcf.com/Article/details/gzkmjystq.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/gifuizdzt.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gkoqkdtag.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gsitgxrre.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/gloqzjtnx.sHtML

name="${1:-default}"
来源：http://blog.vehdjk.com/Article/details/gvtkpbvlh.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gtazoajyl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/geyjawzde.sHtML

[R07] if 判断文件
来源：http://m.share.yfazqb.com/Article/details/giylxwedn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.vehdjk.com/Article/details/geewprxgf.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/gawprkepk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gwqzxeixp.sHtML

[R09] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gsmycfzmu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.bbcook.cn/Article/details/gfvmvxdin.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/goevcevjl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/grzonyvzj.sHtML

[R11] case 多分支
来源：http://3g.tarul.cn/Article/details/gevemaxvo.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/gnhngveju.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/gwntemvea.sHtML

stop)  echo "停止" ;;
来源：http://read.share.yfazqb.com/Article/details/guoyrtdco.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gvdfmadkg.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/gydcexkyc.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/guivuetsh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/gjnjooltw.sHtML

[R13] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gdmtarxsq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gpptfzxjo.sHtML

[R14] C 风格 for
来源：http://www.blog.tarul.cn/Article/details/gqmiwodrz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gmowobzfu.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/ggzaepmhk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gzeklrcnr.sHtML

[R16] until 等待条件
来源：http://read.share.yfazqb.com/Article/details/ginjyftfz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gtmcgeoig.sHtML

[R17] 数组定义与取值
来源：http://m.share.tarul.cn/Article/details/ghrxckvst.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.tarul.cn/Article/details/gbymvtgjd.sHtML

[R18] 遍历数组
来源：http://www.share.sjlbkw.cn/Article/details/gshlksdbo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/gjuldhxpo.sHtML

[R19] 数组长度
来源：http://3g.vehdjk.com/Article/details/gistghfpg.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gspizveot.sHtML

[R20] 关联数组（字典）
来源：http://blog.epnwcf.com/Article/details/gpkmwvuol.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.yfazqb.com/Article/details/gwbjvbgdq.sHtML

[R21] 字符串长度
来源：http://baike.bbcook.cn/Article/details/glapjeznz.sHtML

echo "${#s}"
来源：http://www.blog.fktsv.cn/Article/details/gpngtidjt.sHtML

[R22] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gbmhrhkrq.sHtML

echo "${s:0:5}"
来源：http://www.blog.yfazqb.com/Article/details/gqtqueizn.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/grwywatih.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.tarul.cn/Article/details/gjsnauhjz.sHtML

[R24] 大小写转换
来源：http://baike.fktsv.cn/Article/details/guvcuvhpw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/gzlhuqozv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/gdqkmlzko.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gbkhgmwtp.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gpxdnzxac.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gbvqdgvhi.sHtML

[R27] 算术展开
来源：http://blog.bbcook.cn/Article/details/gzffuriwn.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gwcxnfced.sHtML

[R28] 浮点运算
来源：http://m.share.epnwcf.com/Article/details/gonopldpf.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/gcgholyyp.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/gqugufhgs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/gvtgwyisz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/gkwtboblu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/gyfvlbhxc.sHtML

[R31] 局部变量
来源：http://baike.fktsv.cn/Article/details/gumiehxro.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.epnwcf.com/Article/details/gpdwwdlcp.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/gpzlveerd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/gvowbuoxj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/gjaksegnt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.tarul.cn/Article/details/gwqeiaava.sHtML

[R34] 退出时清理
来源：http://blog.sjlbkw.cn/Article/details/gsxgfilge.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/gkemsyxiy.sHtML

[R35] 后台执行并等待
来源：http://www.blog.epnwcf.com/Article/details/gqznyfrls.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gowskwewi.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.tarul.cn/Article/details/gayelrzkq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/gmhdfzqom.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gwwpbtstt.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/gjtzdfucm.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gwjdzcvzw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gwubvmive.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.yfazqb.com/Article/details/gflsezaxc.sHtML

cmd > out.log 2>&1
来源：http://blog.sjlbkw.cn/Article/details/ghzuarhmw.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/guemadlza.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/gevbijlso.sHtML

[R41] 丢弃输出
来源：http://read.share.fktsv.cn/Article/details/gosgtjgwa.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/gatyrfohb.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/ggfavyoki.sHtML

wc -l < a.txt
来源：http://www.blog.tarul.cn/Article/details/grooleemb.sHtML

[R43] 按名字查找文件
来源：http://mobile.vehdjk.com/Article/details/gbilleeqb.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gjxlkvdrx.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gukpiixgy.sHtML

find . -mtime -7 -type f
来源：http://m.share.vehdjk.com/Article/details/gzeqqjeek.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/gjebwkevs.sHtML

find . -name "*.tmp" -delete
来源：http://3g.vehdjk.com/Article/details/gjlvixmfs.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.epnwcf.com/Article/details/gzgmshkxt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/gwlayubsj.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/gglyaiiuc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fktsv.cn/Article/details/gaiwizxot.sHtML

[R48] awk 取指定列
来源：http://www.blog.tarul.cn/Article/details/gptbsszzg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gezyfdtzq.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gotfuenvn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/gytlxlskd.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/govzsryho.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gydepkasv.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/gtabaicfe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/gwgwvcqdg.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/gmlhpnrwx.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/gxqpiqtvw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/gccbloywz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.epnwcf.com/Article/details/gvjdfpgbg.sHtML

[R54] 比较两个文件
来源：http://www.m.share.tarul.cn/Article/details/gcgskvusz.sHtML

diff a.txt b.txt
来源：http://read.share.fktsv.cn/Article/details/gxgpavbuh.sHtML

[R55] 压缩与解压
来源：http://blog.sjlbkw.cn/Article/details/guscoqidb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/geeglfrcb.sHtML

[R56] 远程拷贝
来源：http://www.blog.bbcook.cn/Article/details/ggwfthtnf.sHtML

scp file user@host:/path/
来源：http://m.share.fktsv.cn/Article/details/gywlmufhx.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/giwfumqoo.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gnemrzsax.sHtML

[R58] 下载文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiwzseuh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.vehdjk.com/Article/details/gpoqftlfa.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/gjdkhveni.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gbdohwfmp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gbzjnxmzz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gircvmczk.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/goklyfwsr.sHtML

df -h;  du -sh *
来源：http://blog.tarul.cn/Article/details/glytgujce.sHtML

[R62] 找最占空间的文件
来源：http://read.share.bbcook.cn/Article/details/gkdjiiupy.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.epnwcf.com/Article/details/gfixkrjyp.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gyjmzxequ.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fktsv.cn/Article/details/gtmkvfojd.sHtML

[R64] 结束进程
来源：http://m.share.bbcook.cn/Article/details/gttjqcskk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.yfazqb.com/Article/details/gfnniykda.sHtML

[R65] 查看端口占用
来源：http://www.share.fktsv.cn/Article/details/grogawldz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/gotonuykh.sHtML

[R66] 定时任务
来源：http://mobile.bbcook.cn/Article/details/gzzyxlzep.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gmwuqmetg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.yfazqb.com/Article/details/gyxplhfeq.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/gpwyvdqix.sHtML

[R68] 计算文件校验值
来源：http://baike.tarul.cn/Article/details/gynwteadh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.yfazqb.com/Article/details/gixgghknq.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gxzshomgu.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.bbcook.cn/Article/details/gmogmhyel.sHtML

[R70] 时间戳与互转
来源：http://www.share.yfazqb.com/Article/details/gprzrkwol.sHtML

date +%s;  date -d @1700000000
来源：http://3g.yfazqb.com/Article/details/ghkrdveog.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gojkgzqdi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gelfqbxbp.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gujecfoqa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gfihtsdtt.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/ggovvzeoc.sHtML

split -l 1000 big.log part_
来源：http://www.blog.bbcook.cn/Article/details/gmsfztmdy.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/gqxwnosay.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.yfazqb.com/Article/details/gpachevft.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gxwlrmevm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.vehdjk.com/Article/details/gakjimamk.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/gvvrekljo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gcjvqdxwv.sHtML

[R77] 读取用户输入
来源：http://mobile.vehdjk.com/Article/details/ggxkevemm.sHtML

read -rp "请输入: " ans
来源：http://wap.tarul.cn/Article/details/ghnbdxktp.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/gqsyywqng.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/gzzufivxa.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gejbzvgaz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/gsigimrbp.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gdtlgtxmz.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gwyjjdfiy.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwgztgybs.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/gtrxszehb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gnnaxywql.sHtML

[S01] C：Hello World
来源：http://wap.tarul.cn/Article/details/gwfsjrorj.sHtML

#include <stdio.h>
来源：http://wap.bbcook.cn/Article/details/gbwbsqozj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fktsv.cn/Article/details/gojufkcix.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/ghmhcyefu.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/gyzkvlrtf.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gwwmcenho.sHtML

int x; scanf("%d", &x);
来源：http://baike.yfazqb.com/Article/details/gfextyyja.sHtML

[S04] C：字符串复制
来源：http://3g.yfazqb.com/Article/details/gqjbnxauf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gxtlpzghi.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/gklvcwmlj.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/gbpcejctp.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/ggksdrhvg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.bbcook.cn/Article/details/gxvnlmjkw.sHtML

[S07] C：数组遍历求和
来源：http://baike.yfazqb.com/Article/details/gzmgymuhx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.sjlbkw.cn/Article/details/gdyyfsonw.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gtegmdzky.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fktsv.cn/Article/details/ghphfsphj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.tarul.cn/Article/details/gafcxmugk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/gaopmvpip.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/grsvcyric.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.yfazqb.com/Article/details/gjvxovati.sHtML

[S11] C：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gmmsjyinx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.epnwcf.com/Article/details/gfoxybqgn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.yfazqb.com/Article/details/gwrxzfabf.sHtML

fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gprrvnsbc.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/gthodcnje.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.epnwcf.com/Article/details/gxltoawpb.sHtML

[S13] C：宏定义
来源：http://mobile.yfazqb.com/Article/details/gavhmdjbq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gswigryzb.sHtML

[S14] C：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gymqhxutj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.vehdjk.com/Article/details/gatfvkmqk.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/gdukyweou.sHtML

(double) a / b
来源：http://m.share.sjlbkw.cn/Article/details/gvhdxfhpx.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gjocjobmg.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/geqirkwsr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gdebibfgl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gacgtgnwv.sHtML

[S18] C：命令行参数
来源：http://www.share.vehdjk.com/Article/details/grruhxtro.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/gvehgrabr.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/griysvmjs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gluqnuyvd.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/gzapvtzhk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gpxfqmrej.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/gjdpmzcry.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.tarul.cn/Article/details/ghoiyvdye.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gxgbasqod.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/ghgbpojbc.sHtML

[S23] C：随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gfssnxlwv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/ggjfhfvzq.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/gqnxyirdq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/guwqfssgk.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gwzexdjcu.sHtML

memcpy(dst, src, n);
来源：http://wap.fktsv.cn/Article/details/gggegzvfs.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/glhoyxvki.sHtML

memset(a, 0, sizeof a);
来源：http://wap.yfazqb.com/Article/details/ganekybla.sHtML

[S27] C：定义常量
来源：http://www.share.vehdjk.com/Article/details/gbhdatioq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gazvxiwii.sHtML

[S28] C：静态变量
来源：http://www.m.share.bbcook.cn/Article/details/gciibbgrh.sHtML

static int counter = 0;
来源：http://3g.vehdjk.com/Article/details/gdrjdzlih.sHtML

[S29] C：变参函数
来源：http://read.share.vehdjk.com/Article/details/gwsmcaknd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gbvsulosk.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/grhtonvdj.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/ghblhtlnl.sHtML

#define X_H
来源：http://mobile.fktsv.cn/Article/details/gnmdbpoyz.sHtML

#endif
来源：http://wap.yfazqb.com/Article/details/gkcjmimfb.sHtML

[S31] C++：Hello World
来源：http://read.share.tarul.cn/Article/details/guolzhizj.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gbofpvicz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fktsv.cn/Article/details/gdbecphwm.sHtML

[S32] C++：字符串
来源：http://wap.epnwcf.com/Article/details/gsnnrcqfi.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/gmhuqhmzu.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gxpvqgqlk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/glztmrozl.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.bbcook.cn/Article/details/gdrvroebf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fktsv.cn/Article/details/gkrorqdqd.sHtML

[S35] C++：map
来源：http://baike.vehdjk.com/Article/details/grhzlkeav.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gfhqrdhda.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.yfazqb.com/Article/details/guwgblauo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gupxcmtdt.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/gyvmxjahs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.tarul.cn/Article/details/ggtmlfxcb.sHtML

[S38] C++：排序
来源：http://www.blog.tarul.cn/Article/details/gvdozldvc.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/gmwhysoli.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/gzyenxpqx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.yfazqb.com/Article/details/glsbwhpoy.sHtML

[S40] C++：查找元素
来源：http://www.share.tarul.cn/Article/details/gbqrglypu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gbvkrdrcu.sHtML


<!-- 参考信息 -->