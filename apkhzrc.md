代发 wailian999

ANALYZE TABLE users;
来源：http://www.blog.bbcook.cn/Article/details/gtgcsgjiq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.sjlbkw.cn/Article/details/gplwoqpzu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gnafhabsh.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/gkzdvrsrn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/gqnrzstvu.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gnrauxzas.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/gggrlzeez.sHtML

[Q74] 强制使用索引
来源：http://baike.vehdjk.com/Article/details/gvtpujjzk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.bbcook.cn/Article/details/gfjenjbip.sHtML

[Q75] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gayykovak.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gbjqrrhfd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gospefnqd.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/gxlpnqbrv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gkqdolxps.sHtML

[Q77] 时间加减
来源：http://mobile.yfazqb.com/Article/details/gzzhzakcv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.bbcook.cn/Article/details/ghjpehqqo.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/gykyjzmjz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.epnwcf.com/Article/details/glehdnxzi.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/ggirqtqqo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.vehdjk.com/Article/details/gsluqmmmn.sHtML

[Q80] 字符串截取
来源：http://read.share.sjlbkw.cn/Article/details/gihlmxvfv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.bbcook.cn/Article/details/gbsmmefiq.sHtML

[Q81] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gtiovadxu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.tarul.cn/Article/details/gzalhwlgm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gmzcxcfpu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gyaxslrra.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gnwnrodae.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/glswcbjtc.sHtML

[Q84] 去除首尾空格
来源：http://blog.yfazqb.com/Article/details/gkprvbpev.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gepirbljz.sHtML

[Q85] 数值取整
来源：http://3g.vehdjk.com/Article/details/ghawhhrqm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.vehdjk.com/Article/details/gbpmtcypx.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/gncgwwedy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.yfazqb.com/Article/details/goblnnqgt.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.bbcook.cn/Article/details/gzutydmqw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.sjlbkw.cn/Article/details/gbizenens.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/gfuhebkyw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.yfazqb.com/Article/details/gyhqqznra.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gqsanghwq.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gfpmhynkx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.bbcook.cn/Article/details/ggresyllg.sHtML

[Q90] 生成序号列
来源：http://mobile.epnwcf.com/Article/details/ggyzhvbyq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.vehdjk.com/Article/details/ghqulsscv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjugenwyi.sHtML

R. Bash 专题
来源：http://www.m.share.fktsv.cn/Article/details/gdjxoifqa.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gidzajvgd.sHtML

[R01] shebang 与严格模式
来源：http://wap.yfazqb.com/Article/details/gscyhzjwq.sHtML

#!/usr/bin/env bash
来源：http://3g.vehdjk.com/Article/details/gbjawtkay.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/gpmtybsir.sHtML

[R02] 变量赋值与使用
来源：http://wap.bbcook.cn/Article/details/gvnqwlmys.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.yfazqb.com/Article/details/gbxzblawa.sHtML

[R03] 只读变量
来源：http://read.share.bbcook.cn/Article/details/gqctjploz.sHtML

readonly PI=3.14
来源：http://m.share.tarul.cn/Article/details/gjuhzwjah.sHtML

[R04] 位置参数
来源：http://read.share.tarul.cn/Article/details/gyxzgzihs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/ggpitkozy.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/gknrvnmph.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/gswltmftd.sHtML

[R06] 判断命令是否存在
来源：http://wap.vehdjk.com/Article/details/gtaulgtup.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/grzkkltjf.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gmtudcubb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.bbcook.cn/Article/details/gqgrqomiw.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/giqqkrqwi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.yfazqb.com/Article/details/giylkxhrs.sHtML

[R09] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/grgefeouw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fktsv.cn/Article/details/gkhpuoaui.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gxzsenxfo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.yfazqb.com/Article/details/gphrpuoif.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/gcaldimxm.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/gkpbqzaqz.sHtML

start) echo "启动" ;;
来源：http://3g.vehdjk.com/Article/details/gluuohtse.sHtML

stop)  echo "停止" ;;
来源：http://baike.vehdjk.com/Article/details/gzbjfddxe.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.epnwcf.com/Article/details/gxbcrbxsd.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/gpqjwfsej.sHtML

[R12] for 遍历文件
来源：http://mobile.vehdjk.com/Article/details/guaapvxxb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.vehdjk.com/Article/details/gnszzawjv.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gdkznpcbp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gpolbeema.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/gkbxwcnsc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/glkjarjly.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gsfmmwdmp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fktsv.cn/Article/details/gwmxjvrxq.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/gntqweawh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gveqbqitr.sHtML

[R17] 数组定义与取值
来源：http://read.share.tarul.cn/Article/details/ggxehrccx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/gwmrehelo.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/geweresmz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.epnwcf.com/Article/details/gxutzywla.sHtML

[R19] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gdbbtfhxj.sHtML

echo "${#arr[@]}"
来源：http://read.share.vehdjk.com/Article/details/guyezdjrs.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/gwqamdwjm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.vehdjk.com/Article/details/grmhowafq.sHtML

[R21] 字符串长度
来源：http://3g.vehdjk.com/Article/details/gwwryguhe.sHtML

echo "${#s}"
来源：http://mobile.fktsv.cn/Article/details/gugpraycu.sHtML

[R22] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/grgnonkwr.sHtML

echo "${s:0:5}"
来源：http://www.share.sjlbkw.cn/Article/details/gqgtzyiuw.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gyyejsnjl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.bbcook.cn/Article/details/genuqytao.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gpwwixlog.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gfanzjaqf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/gygxtxxcr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fktsv.cn/Article/details/gsvdvecvd.sHtML

[R26] 命令替换
来源：http://blog.vehdjk.com/Article/details/gwzadsbzq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.tarul.cn/Article/details/glgqlymmz.sHtML

[R27] 算术展开
来源：http://www.share.epnwcf.com/Article/details/gpacjugeo.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/gtwtbiwsb.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/gjxqwtyki.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.epnwcf.com/Article/details/glotnsguq.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gdeqmycir.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.yfazqb.com/Article/details/geyycfxvj.sHtML

[R30] 函数返回状态码
来源：http://www.share.yfazqb.com/Article/details/gnrlwmrdx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/gzkxuwxhd.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gasbyrcmv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gmigmphji.sHtML

[R32] 参数个数校验
来源：http://read.share.bbcook.cn/Article/details/gpwquzddx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/gkiezmmhr.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.sjlbkw.cn/Article/details/garccsxml.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.yfazqb.com/Article/details/ghliacjek.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/gmqfskhec.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/gvpqvinfj.sHtML

[R35] 后台执行并等待
来源：http://wap.tarul.cn/Article/details/gvzeeapea.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.vehdjk.com/Article/details/gbpnoeabl.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/gpfdkitdz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.epnwcf.com/Article/details/gqoutbact.sHtML

[R37] 把输出赋给变量
来源：http://baike.bbcook.cn/Article/details/goqsggikf.sHtML

files=$(ls -1)
来源：http://blog.tarul.cn/Article/details/gcojdzmpp.sHtML

[R38] 管道串联
来源：http://mobile.sjlbkw.cn/Article/details/gabvtgdvi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/getfbffyw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.epnwcf.com/Article/details/gohrtdejr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/gpqefvaxy.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/gqvwxeouj.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/gebdkoufu.sHtML

[R41] 丢弃输出
来源：http://www.share.bbcook.cn/Article/details/glafvnpag.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gselxjftk.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/gzhifmoss.sHtML

wc -l < a.txt
来源：http://read.share.vehdjk.com/Article/details/gdktvvhvs.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gntousmlq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fktsv.cn/Article/details/guazsdawz.sHtML

[R44] 按修改时间查找
来源：http://www.share.epnwcf.com/Article/details/gncrazxui.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.tarul.cn/Article/details/gckostmgk.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gqhivzias.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.tarul.cn/Article/details/gobchaemm.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/guhqjwyiq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.yfazqb.com/Article/details/gahmsulkf.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrkhuukz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gziehbohh.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/gqrwaznai.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gofntkqcw.sHtML

[R49] awk 带条件
来源：http://baike.tarul.cn/Article/details/gqkvmehej.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.yfazqb.com/Article/details/gptrtyxwv.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/gxscklvmn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.vehdjk.com/Article/details/gpxvvjgpr.sHtML

[R51] 排序去重取前几
来源：http://wap.fktsv.cn/Article/details/gwurprdgr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/gkitrpmnr.sHtML

[R52] 统计行数
来源：http://wap.tarul.cn/Article/details/gksbxrvrt.sHtML

wc -l a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gexemnxxr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/gylhhxbmc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.epnwcf.com/Article/details/gxejhjtkl.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gllnsrbxp.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/gdpvohtys.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/gxuzhnjqy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fktsv.cn/Article/details/gakbkhhmn.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gwkachwue.sHtML

scp file user@host:/path/
来源：http://blog.vehdjk.com/Article/details/gqonxzwpj.sHtML

[R57] 远程执行命令
来源：http://mobile.sjlbkw.cn/Article/details/gzrybanfd.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/gepgdqmwp.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gkugcaalr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/gofzpqqvj.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/grpbfnlil.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.tarul.cn/Article/details/gfxasirft.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gsskawhzv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.epnwcf.com/Article/details/gpdkvrgae.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/guozmjykj.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/gtwtqyjjx.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gjpfahbuz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fktsv.cn/Article/details/gidyyxici.sHtML

[R63] 内存与进程
来源：http://www.blog.yfazqb.com/Article/details/gluqhrvee.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/ggulhrkhe.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/gyzmbsabf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.bbcook.cn/Article/details/geyfenfpl.sHtML

[R65] 查看端口占用
来源：http://www.share.tarul.cn/Article/details/guflfonio.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/gkagetvdf.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gwxyawikv.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/gfefeyvjq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gisxihcjl.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/gzuvlwtno.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/gjpgeeoob.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.yfazqb.com/Article/details/gvdmoarvn.sHtML

[R69] 生成随机密码
来源：http://baike.sjlbkw.cn/Article/details/gqfxtlyzu.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gygotcyja.sHtML

[R70] 时间戳与互转
来源：http://3g.vehdjk.com/Article/details/gqktvgpdi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.epnwcf.com/Article/details/gpxandoec.sHtML

[R71] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gnzpheadc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gwaojnzuz.sHtML

[R72] 等待端口就绪
来源：http://mobile.yfazqb.com/Article/details/ghjkzenwm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gzyyhatsk.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/gdqzgcavh.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/gposfooex.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/gkbxxlwvt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gxescxljr.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/gsdvutzwv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.yfazqb.com/Article/details/gflgndeua.sHtML

[R76] 使用临时文件
来源：http://m.share.yfazqb.com/Article/details/grsofnnsq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/gvmdxpxgx.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gxfxvvmsf.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/gfkqafdfl.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/grzkonfqj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fktsv.cn/Article/details/gckjcffzo.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/gnzwqeeaj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.epnwcf.com/Article/details/gaemxupdb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.sjlbkw.cn/Article/details/gvqscbbbe.sHtML

time ./run.sh
来源：http://www.m.share.vehdjk.com/Article/details/gyjjtdxgn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gixrbgtfd.sHtML

S. C / C++ 专题
来源：http://wap.epnwcf.com/Article/details/gcxdelhmp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdtxmxchj.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gvyzejehi.sHtML

#include <stdio.h>
来源：http://blog.vehdjk.com/Article/details/gyswleizl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.yfazqb.com/Article/details/gxasqxmns.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.epnwcf.com/Article/details/gvshnzaxn.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/gldpdhcdf.sHtML

[S03] C：读入整数
来源：http://3g.sjlbkw.cn/Article/details/gquwcxkua.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/glgyrkvke.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/gluhfmnul.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.yfazqb.com/Article/details/gnzoozsrb.sHtML

[S05] C：字符串长度
来源：http://mobile.tarul.cn/Article/details/gectsikvy.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/gphyysdeo.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/gaiwinxjx.sHtML

strcmp(a, b) == 0
来源：http://blog.epnwcf.com/Article/details/gzzsdqlhs.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gthudqwcb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.bbcook.cn/Article/details/giwtqzltb.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gplvgqoko.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gwqyeonjv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.yfazqb.com/Article/details/gdjxtkoki.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.yfazqb.com/Article/details/goaxgdpsk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gisrahuua.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/grkkvhfnu.sHtML

[S11] C：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gjallytep.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.yfazqb.com/Article/details/gijbybmuv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.vehdjk.com/Article/details/gcmozptav.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/geckpwuqm.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/gjtvlvstd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gisdcbgco.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/gflzphxbi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gxhaxojgv.sHtML

[S14] C：枚举
来源：http://blog.vehdjk.com/Article/details/gskjqxoug.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.tarul.cn/Article/details/gcpejfvgj.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/gvtjyctrx.sHtML

(double) a / b
来源：http://wap.tarul.cn/Article/details/gofemiyqw.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/grgcqusbj.sHtML

x |= (1 << 3);
来源：http://m.share.bbcook.cn/Article/details/gvecmlxzw.sHtML

[S17] C：安全拼接字符串
来源：http://3g.vehdjk.com/Article/details/gquettjeo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.vehdjk.com/Article/details/gpqulgted.sHtML

[S18] C：命令行参数
来源：http://read.share.epnwcf.com/Article/details/gwjidbqsk.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gcydytpph.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/gkwkoeyfr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gacegzkjo.sHtML

[S20] C：二分查找
来源：http://mobile.fktsv.cn/Article/details/gkotdgukj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gcqgpcwjm.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/grpbbhzen.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.yfazqb.com/Article/details/gtjjnwplk.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gkutnzdep.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/ggpblaxeb.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/gpptnfdsi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.sjlbkw.cn/Article/details/gmdpetrzv.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gtnbliyay.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/gkjbpqjkq.sHtML

[S25] C：内存拷贝
来源：http://read.share.tarul.cn/Article/details/grvnuaiqf.sHtML

memcpy(dst, src, n);
来源：http://m.share.vehdjk.com/Article/details/gapfkkazg.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/gytrcmjbf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fktsv.cn/Article/details/ggrxndjmi.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gggooaiuu.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gcleqvmti.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gosgmnszr.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/gpbvaebzy.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/gizhegdmo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.yfazqb.com/Article/details/guwrcalfx.sHtML

[S30] C：头文件保护
来源：http://wap.tarul.cn/Article/details/gxijptctw.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gybpcjqzp.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/gozjxekbk.sHtML

#endif
来源：http://wap.tarul.cn/Article/details/gmbpstsvx.sHtML

[S31] C++：Hello World
来源：http://wap.yfazqb.com/Article/details/gdpvymsde.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/gzcecdmzh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/grwuicjao.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/gcyyieoqr.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gzxwcnczl.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.tarul.cn/Article/details/gdzjxbons.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.bbcook.cn/Article/details/gmxfvmbbt.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/gdbxqsdec.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.epnwcf.com/Article/details/gmsivpojw.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/glijpyiwg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gjojytkgw.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/gfgrojidb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gnnszekpa.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/glupqdnfg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.yfazqb.com/Article/details/gliplpscr.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gsrihleyj.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/guzuidsox.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.yfazqb.com/Article/details/gogphrsqd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/grgguhohr.sHtML

[S40] C++：查找元素
来源：http://blog.vehdjk.com/Article/details/ggjiogbfr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/gmjepogns.sHtML


<!-- 参考信息 -->