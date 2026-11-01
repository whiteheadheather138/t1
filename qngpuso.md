代发 wailian999

SHOW INDEX FROM users;
来源：http://mobile.bbcook.cn/Article/details/gltlvqqfy.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/gfikytzxz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/gbhoputft.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gtrxsocep.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbkbqgvh.sHtML

[Q75] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gpnbaanpk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/gvpbfenli.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/gnaafsszh.sHtML

[Q76] 按天统计
来源：http://www.blog.bbcook.cn/Article/details/gushsizsb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.epnwcf.com/Article/details/ghewyorwg.sHtML

[Q77] 时间加减
来源：http://www.share.sjlbkw.cn/Article/details/gmyfsmqhc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.yfazqb.com/Article/details/guymheyuh.sHtML

[Q78] 当前时间
来源：http://www.blog.yfazqb.com/Article/details/garhdxpiz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.vehdjk.com/Article/details/gkqgzsvwl.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/gtugoaubw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.epnwcf.com/Article/details/gqmkkkcgw.sHtML

[Q80] 字符串截取
来源：http://3g.tarul.cn/Article/details/gefbodzqi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.tarul.cn/Article/details/gqzdoixih.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gxleaxfmq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/guvemjhbp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.sjlbkw.cn/Article/details/guqznrbas.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gdrubfgxp.sHtML

[Q83] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gncgmpzto.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gjgobajkh.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.epnwcf.com/Article/details/guhiccovw.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gqusieutv.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/gffpvqxtl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.epnwcf.com/Article/details/gcknyeeai.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.tarul.cn/Article/details/grbdwxokn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.yfazqb.com/Article/details/govosjxsq.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.vehdjk.com/Article/details/gcamdrvra.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/gjatkgipx.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.yfazqb.com/Article/details/gtnfiwfsu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.tarul.cn/Article/details/guhigmpkw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.tarul.cn/Article/details/gqikdgwze.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/giakmjxur.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gijgseanm.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gzrxtxcow.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/gipotdfod.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gpsqdbpve.sHtML

R. Bash 专题
来源：http://www.blog.vehdjk.com/Article/details/gtejskfkz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwmkewceg.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.tarul.cn/Article/details/ggkktafyy.sHtML

#!/usr/bin/env bash
来源：http://wap.yfazqb.com/Article/details/gedugmwzg.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gzqlmulej.sHtML

[R02] 变量赋值与使用
来源：http://www.share.bbcook.cn/Article/details/gyooksjci.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.yfazqb.com/Article/details/gvfgwwvbu.sHtML

[R03] 只读变量
来源：http://blog.bbcook.cn/Article/details/gjptyjpbm.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gukdyyhme.sHtML

[R04] 位置参数
来源：http://mobile.tarul.cn/Article/details/gimofvtpz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.sjlbkw.cn/Article/details/gmuqcjxyq.sHtML

[R05] 参数默认值
来源：http://read.share.yfazqb.com/Article/details/gqgxcccxt.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/galecnmgx.sHtML

[R06] 判断命令是否存在
来源：http://baike.yfazqb.com/Article/details/gkgknkdjr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gsiqetsur.sHtML

[R07] if 判断文件
来源：http://www.blog.yfazqb.com/Article/details/gdwhwzaez.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.epnwcf.com/Article/details/gwzewiiwa.sHtML

[R08] 数值比较
来源：http://www.m.share.tarul.cn/Article/details/gcxteaiyn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/gmmfzuwsc.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gcpukciwu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.sjlbkw.cn/Article/details/ggpfyenqm.sHtML

[R10] 正则匹配
来源：http://blog.vehdjk.com/Article/details/gkgjdtuvb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/giryzhuhp.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gmclfnzuz.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/gymdxruhk.sHtML

start) echo "启动" ;;
来源：http://www.share.tarul.cn/Article/details/gkaqymmja.sHtML

stop)  echo "停止" ;;
来源：http://blog.bbcook.cn/Article/details/gzboeudkb.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/ginorhpqp.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/gcolythef.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gnfystmwo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gvqpdpxmm.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/grhhfnyuk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gvkfnzqph.sHtML

[R14] C 风格 for
来源：http://baike.vehdjk.com/Article/details/gcrcjssrm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gnkkejlrf.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gsgtonncz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/gsjapepev.sHtML

[R16] until 等待条件
来源：http://m.share.yfazqb.com/Article/details/gyudgtvhx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/ggmglnmgk.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/ghikeweiu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.epnwcf.com/Article/details/gxthgycky.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/gyojwavyn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gwjsczffa.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gxwodjzfi.sHtML

echo "${#arr[@]}"
来源：http://baike.bbcook.cn/Article/details/gutskvgoj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/ggtxhxiio.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gsshvbxfa.sHtML

[R21] 字符串长度
来源：http://baike.bbcook.cn/Article/details/gdrkqkpru.sHtML

echo "${#s}"
来源：http://baike.yfazqb.com/Article/details/glaoaoyfd.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gllcmldgl.sHtML

echo "${s:0:5}"
来源：http://mobile.epnwcf.com/Article/details/grnitbzzj.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/ggrzpqpol.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.yfazqb.com/Article/details/giytdvdgc.sHtML

[R24] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gdmiiqyeg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.sjlbkw.cn/Article/details/gqycglvhm.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.yfazqb.com/Article/details/gmylqhkkb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.epnwcf.com/Article/details/gpnuenftq.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/gwizanyyk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.yfazqb.com/Article/details/gnzovdwif.sHtML

[R27] 算术展开
来源：http://m.share.vehdjk.com/Article/details/gvkzoyoga.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/gzphtivnb.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/gobkboszj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.yfazqb.com/Article/details/gqewyciio.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gyvkkquaz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.vehdjk.com/Article/details/gxqqajodu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkbuixxu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gpwdgyjtv.sHtML

[R31] 局部变量
来源：http://blog.sjlbkw.cn/Article/details/girdakymx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gesjeezdu.sHtML

[R32] 参数个数校验
来源：http://mobile.sjlbkw.cn/Article/details/gldfnrnld.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/giweacoki.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gvsfcnvdq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/gwktqqilo.sHtML

[R34] 退出时清理
来源：http://3g.fktsv.cn/Article/details/gorlqguya.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gzkrmhfgx.sHtML

[R35] 后台执行并等待
来源：http://blog.yfazqb.com/Article/details/gcuqkrxfg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fktsv.cn/Article/details/glxpkjvbh.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gwsuatkoy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.sjlbkw.cn/Article/details/gtrxinnuj.sHtML

[R37] 把输出赋给变量
来源：http://baike.sjlbkw.cn/Article/details/gveeyxcxo.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/gwzsjxgfn.sHtML

[R38] 管道串联
来源：http://www.blog.sjlbkw.cn/Article/details/gdxfstqbl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.vehdjk.com/Article/details/gbzwbcohw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.vehdjk.com/Article/details/ghggwofzd.sHtML

cmd > out.log 2>&1
来源：http://www.share.vehdjk.com/Article/details/gseizuluv.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/ghewehdwu.sHtML

echo "log" >> out.log
来源：http://read.share.bbcook.cn/Article/details/gjqnvexkh.sHtML

[R41] 丢弃输出
来源：http://baike.vehdjk.com/Article/details/gryzlwnlo.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gvzqyqhvg.sHtML

[R42] 输入重定向
来源：http://wap.tarul.cn/Article/details/ghsppdxzu.sHtML

wc -l < a.txt
来源：http://3g.vehdjk.com/Article/details/gizbghzrz.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gjrklewnn.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gierhgzjs.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/ghgvixnom.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/ggupohwyd.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/gyfmyprwh.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fktsv.cn/Article/details/gjbonkeft.sHtML

[R46] 递归替换文件内容
来源：http://www.share.vehdjk.com/Article/details/ghnbhoxtn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/gpsjszzcy.sHtML

[R47] sed 单行替换
来源：http://baike.vehdjk.com/Article/details/gbnimabpy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.yfazqb.com/Article/details/gtjcodpnr.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gsegtatsv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gufcuptof.sHtML

[R49] awk 带条件
来源：http://www.share.vehdjk.com/Article/details/giajqnygs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gmefvchar.sHtML

[R50] awk 求和
来源：http://mobile.yfazqb.com/Article/details/gnfihhcwj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/gyerbksza.sHtML

[R51] 排序去重取前几
来源：http://mobile.bbcook.cn/Article/details/gpvwamgqu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gpgaawtxk.sHtML

[R52] 统计行数
来源：http://baike.yfazqb.com/Article/details/gdyfkyoht.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gnnxbkbsu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.yfazqb.com/Article/details/ggxmspxqa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gsdscvefu.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/glplmdded.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/govnmcxqw.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/gtqzpoufy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/gqkvmgqoq.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/gcqcdneae.sHtML

scp file user@host:/path/
来源：http://blog.yfazqb.com/Article/details/gzqnomqha.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/gpbticdqk.sHtML

ssh user@host 'uptime'
来源：http://mobile.bbcook.cn/Article/details/gyvxciafy.sHtML

[R58] 下载文件
来源：http://3g.epnwcf.com/Article/details/gkvmpocct.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gifosfoha.sHtML

[R59] 发 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gahksmnnl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.bbcook.cn/Article/details/gshavngcm.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/ghhpeuopt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/golaeiqnh.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fktsv.cn/Article/details/gfnhlddoa.sHtML

df -h;  du -sh *
来源：http://wap.fktsv.cn/Article/details/gzvyurooi.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/gtezozgwr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gkvkifyns.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gtjpplqqt.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.bbcook.cn/Article/details/gfkoipvdi.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/gdtlfgmoo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.epnwcf.com/Article/details/grnidxgyw.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/gtypjlnka.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.yfazqb.com/Article/details/ggvorbnul.sHtML

[R66] 定时任务
来源：http://3g.yfazqb.com/Article/details/gltcpiwvi.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gmbjiaokl.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gzsiahndi.sHtML

openssl rand -hex 16
来源：http://www.blog.fktsv.cn/Article/details/gftlbmyfd.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/ggaykovxr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/guthzsudh.sHtML

[R69] 生成随机密码
来源：http://www.m.share.sjlbkw.cn/Article/details/gpymprqsk.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/gdzuleiub.sHtML

[R70] 时间戳与互转
来源：http://www.share.yfazqb.com/Article/details/gupbfvasi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.tarul.cn/Article/details/gttjufsyx.sHtML

[R71] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gfkubqdna.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fktsv.cn/Article/details/gsswugglc.sHtML

[R72] 等待端口就绪
来源：http://blog.bbcook.cn/Article/details/gchleaxgj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gmljamtfp.sHtML

[R73] 分割大日志
来源：http://3g.sjlbkw.cn/Article/details/gxshkaurr.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/ggwnytkhb.sHtML

[R74] 批量重命名
来源：http://baike.tarul.cn/Article/details/gcmsuodbu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gqsyeyvtb.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gdnrskimd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/gseysnocr.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fktsv.cn/Article/details/gmzxgzmpl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gbikatmma.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gnykvcajh.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/gqaxyhdwd.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gonfetomi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.sjlbkw.cn/Article/details/gxwcgsxbv.sHtML

[R79] 解析命令行选项
来源：http://mobile.fktsv.cn/Article/details/gwndsfksv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/gjlfymilu.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.yfazqb.com/Article/details/gclzmktqm.sHtML

time ./run.sh
来源：http://m.share.tarul.cn/Article/details/ghffodgmc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gtrxwmxxp.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gmzuwreee.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gznvgjswe.sHtML

[S01] C：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gxbjzuofc.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/gpcgjutyp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gmhkfoaps.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/geunvombe.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.tarul.cn/Article/details/gynnckflc.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gopwdizun.sHtML

int x; scanf("%d", &x);
来源：http://blog.epnwcf.com/Article/details/gjvbqplpf.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/ggzhmlknv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/ghuouimqk.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/giywlhwcm.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/gcvtlkzki.sHtML

[S06] C：字符串比较
来源：http://www.share.epnwcf.com/Article/details/glzktzngw.sHtML

strcmp(a, b) == 0
来源：http://3g.yfazqb.com/Article/details/gafbnxvdw.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fktsv.cn/Article/details/gamaieoyc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.bbcook.cn/Article/details/gvdqqnpzf.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.tarul.cn/Article/details/gavuuzmun.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gbtpzrmlv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/gkfgwmehy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/glhslmnrr.sHtML

[S10] C：指针与解引用
来源：http://wap.tarul.cn/Article/details/gtypxthww.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/gpgpimbhm.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/govaaplnm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fktsv.cn/Article/details/gnucjpkuk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.tarul.cn/Article/details/gmazdmppt.sHtML

fclose(f);
来源：http://m.share.tarul.cn/Article/details/gkmaoitwe.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/goqtjswmu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gjutnntmv.sHtML

[S13] C：宏定义
来源：http://www.blog.sjlbkw.cn/Article/details/gervupgsj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/gmudvmkxd.sHtML

[S14] C：枚举
来源：http://baike.yfazqb.com/Article/details/gglssulna.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.vehdjk.com/Article/details/gzllmdlyj.sHtML

[S15] C：类型转换
来源：http://www.blog.vehdjk.com/Article/details/gtgkhmeax.sHtML

(double) a / b
来源：http://m.share.epnwcf.com/Article/details/gdmurtxvw.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/gwvanlyau.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/gunzufozz.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gpluloszo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.sjlbkw.cn/Article/details/gbmdoyfte.sHtML

[S18] C：命令行参数
来源：http://baike.bbcook.cn/Article/details/gjuutohnc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fktsv.cn/Article/details/gcjnirkoz.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/gwqjmqckr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gqzooegil.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gvpmszheo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/glwkabajc.sHtML

[S21] C：字符类别判断
来源：http://blog.fktsv.cn/Article/details/gehcjqzjn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/gxxtwzmpk.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gxngjvmue.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/guehlbygm.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/gguwvsmmg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/guuvzwcmc.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/gnrglvvqi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gjdbvdcwv.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gngspqtrr.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/gcrkmsvxf.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/gxlajruzj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.epnwcf.com/Article/details/gxvpctzms.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/gohfseith.sHtML

const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/ghqndilra.sHtML

[S28] C：静态变量
来源：http://wap.epnwcf.com/Article/details/gqhtlopcr.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/gnbzcedml.sHtML

[S29] C：变参函数
来源：http://www.share.tarul.cn/Article/details/gjyhbdmdg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gfyfouwia.sHtML

[S30] C：头文件保护
来源：http://read.share.bbcook.cn/Article/details/gyirlleag.sHtML

#ifndef X_H
来源：http://baike.vehdjk.com/Article/details/gbrbaguob.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/gcxheymwy.sHtML

#endif
来源：http://www.share.epnwcf.com/Article/details/gnlhvxttn.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/gqpaxkpti.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/glgkxlroj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.epnwcf.com/Article/details/gdzqvnlig.sHtML

[S32] C++：字符串
来源：http://mobile.tarul.cn/Article/details/gkenqyjin.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.yfazqb.com/Article/details/gdzdgrslg.sHtML

[S33] C++：vector 增删
来源：http://blog.tarul.cn/Article/details/grlnswzqz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/gvyiogdfq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/ghbkmrtis.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.vehdjk.com/Article/details/gghanfdhq.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gzuhkmkpy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gofmpvzqj.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/gvykqrjzm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gseebvyym.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/ganrvcjkn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fktsv.cn/Article/details/gkjfyvldx.sHtML

[S38] C++：排序
来源：http://www.m.share.bbcook.cn/Article/details/gfkptfnkv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.yfazqb.com/Article/details/glebvfgkj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.epnwcf.com/Article/details/gxaalcmes.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/gutafjqns.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gghmxuyba.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.sjlbkw.cn/Article/details/ghfkjscpf.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gbbilnzkm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/gubuvqjil.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.epnwcf.com/Article/details/gpbtwgfhu.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.yfazqb.com/Article/details/grebffqnb.sHtML


<!-- 参考信息 -->