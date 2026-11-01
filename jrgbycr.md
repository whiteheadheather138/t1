代发 wailian999

[Q65] 回滚事务
来源：http://read.share.yfazqb.com/Article/details/gkppholuf.sHtML

ROLLBACK;
来源：http://baike.tarul.cn/Article/details/gduajhidg.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gmvfjvtti.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.yfazqb.com/Article/details/gpbwkjopj.sHtML

[Q67] 设置隔离级别
来源：http://wap.yfazqb.com/Article/details/gbqrjjnyn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/grgibcmfm.sHtML

[Q68] 保存点
来源：http://www.m.share.bbcook.cn/Article/details/gduxszmie.sHtML

SAVEPOINT sp1;
来源：http://mobile.bbcook.cn/Article/details/gfkmuqzql.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gvwowakup.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gnchhlpyy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.tarul.cn/Article/details/gvftzwoea.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.bbcook.cn/Article/details/gqdjprubt.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtacsfcw.sHtML

[Q71] 查看建表语句
来源：http://wap.epnwcf.com/Article/details/gbrkkwzpx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/glzhjglfi.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gdlnzyljp.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gkdkebikj.sHtML

[Q73] 查看表状态
来源：http://www.blog.bbcook.cn/Article/details/gbcrokifq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.tarul.cn/Article/details/gkcnehlay.sHtML

[Q74] 强制使用索引
来源：http://read.share.sjlbkw.cn/Article/details/girykucqe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.yfazqb.com/Article/details/gainwpfar.sHtML

[Q75] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gtneblpet.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gfysildsn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gnopujjip.sHtML

[Q76] 按天统计
来源：http://www.share.tarul.cn/Article/details/gzkrnisyb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.sjlbkw.cn/Article/details/gwgbqmmof.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/gvyznglnq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.vehdjk.com/Article/details/gzbjuyoqu.sHtML

[Q78] 当前时间
来源：http://www.blog.epnwcf.com/Article/details/gyltxthcr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.vehdjk.com/Article/details/grnsuqznz.sHtML

[Q79] 字符串拼接
来源：http://blog.tarul.cn/Article/details/gtpnjsvwa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/gdjztddgp.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/gshkyurqk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/getucbkyc.sHtML

[Q81] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gpxumcnvx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fktsv.cn/Article/details/gnwaqnqsi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fktsv.cn/Article/details/glievpftk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/grytyubcs.sHtML

[Q83] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/goovczwqt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/ggxzwkdhw.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/gizuvnbce.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gklywqloj.sHtML

[Q85] 数值取整
来源：http://blog.vehdjk.com/Article/details/gamwjtmtk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gslvatjtd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gsmvmywpa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/gbukuzihk.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gdesdyzxz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gepacbdoi.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.vehdjk.com/Article/details/ghujcvixr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/gkmemwpoy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.epnwcf.com/Article/details/gwlnobbtg.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gnxvfubrk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.epnwcf.com/Article/details/gnwdntgwe.sHtML

[Q90] 生成序号列
来源：http://3g.vehdjk.com/Article/details/gzofqoqcc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/govemfsuf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxqibmllc.sHtML

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/gmaitywzw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxcrqybms.sHtML

[R01] shebang 与严格模式
来源：http://wap.vehdjk.com/Article/details/gampaljwg.sHtML

#!/usr/bin/env bash
来源：http://m.share.yfazqb.com/Article/details/gbonosrtj.sHtML

set -euo pipefail
来源：http://blog.tarul.cn/Article/details/gjbhjpmau.sHtML

[R02] 变量赋值与使用
来源：http://read.share.bbcook.cn/Article/details/gtjatccca.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fktsv.cn/Article/details/gblyyxcbo.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/guoezsrkg.sHtML

readonly PI=3.14
来源：http://www.share.tarul.cn/Article/details/gkiwhdyyy.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/gbnyirhgz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fktsv.cn/Article/details/gpftdbmhu.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/gysumhgwa.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/gqijzgndn.sHtML

[R06] 判断命令是否存在
来源：http://read.share.yfazqb.com/Article/details/girpchydp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gxobeysep.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/gyyychiiv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.vehdjk.com/Article/details/grdvrofgv.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/gutdjldxp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.sjlbkw.cn/Article/details/guxzzzzjm.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gtdqwgvrk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fktsv.cn/Article/details/gozvuscyb.sHtML

[R10] 正则匹配
来源：http://3g.yfazqb.com/Article/details/gvwhyvjrw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.vehdjk.com/Article/details/gtazydzwk.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/gzbixdgmo.sHtML

case "$1" in
来源：http://read.share.yfazqb.com/Article/details/gaapedddq.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/ggkcsgcve.sHtML

stop)  echo "停止" ;;
来源：http://3g.fktsv.cn/Article/details/guhimurkv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gjiipkwqp.sHtML

esac
来源：http://www.share.yfazqb.com/Article/details/gufegzobr.sHtML

[R12] for 遍历文件
来源：http://www.blog.epnwcf.com/Article/details/gxcvswadl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/gujmqxwvn.sHtML

[R13] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gvxxtfush.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/glfvenrrv.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/gdiuxzffr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gcmhndrms.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gfecmyjrm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/grmrkbpzq.sHtML

[R16] until 等待条件
来源：http://www.m.share.yfazqb.com/Article/details/gndikyelv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gwagytmmi.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/gmkzvaznu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gqnvgmnzk.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gtlyuodwg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.tarul.cn/Article/details/ggtguonbz.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/giywvotri.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gkqcodqgz.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/ggbouxjot.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/grjqiqdzs.sHtML

[R21] 字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gmgrbdrls.sHtML

echo "${#s}"
来源：http://www.m.share.vehdjk.com/Article/details/gltxxtnei.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/ghzxbzzpl.sHtML

echo "${s:0:5}"
来源：http://baike.tarul.cn/Article/details/ghhopdscw.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gqnxjtped.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/gakprtpls.sHtML

[R24] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gcgflgncd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/gwwvodcjg.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gachmvbif.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fktsv.cn/Article/details/gypowqqmj.sHtML

[R26] 命令替换
来源：http://m.share.sjlbkw.cn/Article/details/gyjpqawuf.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.epnwcf.com/Article/details/gagvjmjmd.sHtML

[R27] 算术展开
来源：http://blog.epnwcf.com/Article/details/gdutsbutt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fktsv.cn/Article/details/gklvgruqx.sHtML

[R28] 浮点运算
来源：http://wap.sjlbkw.cn/Article/details/ghitonffh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.vehdjk.com/Article/details/glqzlsvqi.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gqgvlgsdz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.tarul.cn/Article/details/gzmdsgtha.sHtML

[R30] 函数返回状态码
来源：http://3g.tarul.cn/Article/details/giurdrtkt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.yfazqb.com/Article/details/gofdwyqik.sHtML

[R31] 局部变量
来源：http://www.blog.yfazqb.com/Article/details/gksypwrvd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpetyhuhf.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/grnwbkhbn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gofqwogwa.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fktsv.cn/Article/details/gnfwwcndn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.epnwcf.com/Article/details/glzrhwwoj.sHtML

[R34] 退出时清理
来源：http://www.m.share.vehdjk.com/Article/details/gheaemdhf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gckuqpgib.sHtML

[R35] 后台执行并等待
来源：http://3g.epnwcf.com/Article/details/gpezkkguw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.bbcook.cn/Article/details/grvpbdqvw.sHtML

[R36] 并发执行多个任务
来源：http://wap.epnwcf.com/Article/details/gpfkyfnbb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/ghimpnzhe.sHtML

[R37] 把输出赋给变量
来源：http://3g.epnwcf.com/Article/details/gppaavhfk.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/gtugmektd.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/gtckgztdm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gqoergusc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.bbcook.cn/Article/details/gmzxwiwkx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gfcawgsjc.sHtML

[R40] 追加写日志
来源：http://blog.yfazqb.com/Article/details/gaeulgkmb.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/gfpfzyefp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gorpxglxr.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/gmnrsjlxe.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gmexeewfq.sHtML

wc -l < a.txt
来源：http://mobile.epnwcf.com/Article/details/gvadisvuj.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fktsv.cn/Article/details/gwkgjcvzq.sHtML

find . -name "*.log" -type f
来源：http://read.share.sjlbkw.cn/Article/details/ggfdrwlij.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/gyqarzkdi.sHtML

find . -mtime -7 -type f
来源：http://www.blog.bbcook.cn/Article/details/gqpipnzyq.sHtML

[R45] 批量删除
来源：http://read.share.fktsv.cn/Article/details/gezdfsxnt.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.sjlbkw.cn/Article/details/gcghykmas.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.epnwcf.com/Article/details/gznvdpbvo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.bbcook.cn/Article/details/geyhyfisk.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fktsv.cn/Article/details/gsbjyvznz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.bbcook.cn/Article/details/gyrfbmwuu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.bbcook.cn/Article/details/gpfastspa.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gctauqpgz.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/grcaryypv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/glewbxbid.sHtML

[R50] awk 求和
来源：http://baike.yfazqb.com/Article/details/gfmrakkre.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.tarul.cn/Article/details/gosinquqz.sHtML

[R51] 排序去重取前几
来源：http://mobile.sjlbkw.cn/Article/details/gurvhujtu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.vehdjk.com/Article/details/gblsliovy.sHtML

[R52] 统计行数
来源：http://blog.fktsv.cn/Article/details/gzffwwfjj.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gdumbiceg.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.tarul.cn/Article/details/gqkjzizrt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.epnwcf.com/Article/details/gajdylfxj.sHtML

[R54] 比较两个文件
来源：http://baike.epnwcf.com/Article/details/gfyjxnwsd.sHtML

diff a.txt b.txt
来源：http://www.blog.fktsv.cn/Article/details/gwsnortis.sHtML

[R55] 压缩与解压
来源：http://mobile.tarul.cn/Article/details/gjsnvejsi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.yfazqb.com/Article/details/gomvlmasi.sHtML

[R56] 远程拷贝
来源：http://mobile.tarul.cn/Article/details/ghdeshdpf.sHtML

scp file user@host:/path/
来源：http://baike.vehdjk.com/Article/details/gpitxroim.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/gfpolcfcn.sHtML

ssh user@host 'uptime'
来源：http://blog.vehdjk.com/Article/details/gmqiifwed.sHtML

[R58] 下载文件
来源：http://baike.tarul.cn/Article/details/gtjqzybvm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.sjlbkw.cn/Article/details/gcjamytmn.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gdgokaayq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.bbcook.cn/Article/details/gcrlewnco.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/ggheqfjtb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.yfazqb.com/Article/details/grkewuuyh.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gbmxxdamu.sHtML

df -h;  du -sh *
来源：http://wap.yfazqb.com/Article/details/gidbhruer.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/glwkadbdb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.yfazqb.com/Article/details/guojovapm.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/gqvkcpwte.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gushfbpbl.sHtML

[R64] 结束进程
来源：http://mobile.yfazqb.com/Article/details/gdeskrdcf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.yfazqb.com/Article/details/gmxodydev.sHtML

[R65] 查看端口占用
来源：http://wap.fktsv.cn/Article/details/gdwjtqzdv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gghruzdru.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/gqfsropsc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.yfazqb.com/Article/details/gmqpzsdjr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gbksjplng.sHtML

openssl rand -hex 16
来源：http://wap.vehdjk.com/Article/details/gcobalwxi.sHtML

[R68] 计算文件校验值
来源：http://wap.vehdjk.com/Article/details/gdmptqijj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.vehdjk.com/Article/details/gkqkdkayn.sHtML

[R69] 生成随机密码
来源：http://m.share.sjlbkw.cn/Article/details/gbcxlaklz.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gkzkrbzyd.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gsgxdgrek.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fktsv.cn/Article/details/glsgnkifk.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gcqzuzizc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fktsv.cn/Article/details/grgihtrbt.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/gueopqqgt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gzfqkiwbi.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gligqdcdy.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gldapwlts.sHtML

[R74] 批量重命名
来源：http://m.share.bbcook.cn/Article/details/ghivreiqw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.vehdjk.com/Article/details/gddqnpwry.sHtML

[R75] 导出环境变量
来源：http://mobile.vehdjk.com/Article/details/gcdatmfgq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fktsv.cn/Article/details/gktuorria.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/ggnvfwdcc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gcocnqdoo.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/gvybfekat.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gpilbuqkh.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/gdzndtliw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/gipspixdt.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gxubrbaxh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/gfjovewcg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/gjknidxha.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/gikpujhgz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gboqxnfjg.sHtML

S. C / C++ 专题
来源：http://wap.sjlbkw.cn/Article/details/gvamsjijn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtxrzwwpl.sHtML

[S01] C：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gpqbzmsjn.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/glztldyap.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.tarul.cn/Article/details/grsqxrnuh.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/guffakbag.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.yfazqb.com/Article/details/glhvzurjv.sHtML

[S03] C：读入整数
来源：http://m.share.yfazqb.com/Article/details/gbceijiim.sHtML

int x; scanf("%d", &x);
来源：http://blog.epnwcf.com/Article/details/gaqtorkyb.sHtML

[S04] C：字符串复制
来源：http://3g.vehdjk.com/Article/details/gtercktan.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fktsv.cn/Article/details/gmnvipzne.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/gwfbyzrwl.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/gjdqmrzcv.sHtML

[S06] C：字符串比较
来源：http://www.share.vehdjk.com/Article/details/gmadaokik.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/gmaprcufp.sHtML

[S07] C：数组遍历求和
来源：http://3g.tarul.cn/Article/details/gmspweuhk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.sjlbkw.cn/Article/details/gamzdtaxn.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.epnwcf.com/Article/details/govrqbidv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.bbcook.cn/Article/details/gfjvappxq.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.vehdjk.com/Article/details/gkbbrbacq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.bbcook.cn/Article/details/gnsmayeoa.sHtML

[S10] C：指针与解引用
来源：http://read.share.tarul.cn/Article/details/gcgwcpyob.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gokylykjp.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gkweytoya.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.vehdjk.com/Article/details/gaznfhmcv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fktsv.cn/Article/details/guigbvmer.sHtML

fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gscfgeumy.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/giuvabpak.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.tarul.cn/Article/details/gbeelhkvu.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/gpzoyfycq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/gfgmjchqg.sHtML

[S14] C：枚举
来源：http://wap.fktsv.cn/Article/details/gpvsifgrb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/gyjdurfah.sHtML

[S15] C：类型转换
来源：http://m.share.tarul.cn/Article/details/gmhgpktze.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/gsnjbawkp.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gkukpjdzb.sHtML

x |= (1 << 3);
来源：http://m.share.fktsv.cn/Article/details/guxgypqco.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/gnuybjfea.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.vehdjk.com/Article/details/gqakbrbya.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoplfgxp.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gyumhyoba.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gbpfryunm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gterqvpky.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/gphmitnrp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gaozllxfr.sHtML

[S21] C：字符类别判断
来源：http://mobile.tarul.cn/Article/details/gxoopsrtr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.yfazqb.com/Article/details/gizkheywo.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gvzlguixf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.vehdjk.com/Article/details/grsykrnfa.sHtML

[S23] C：随机数
来源：http://www.share.vehdjk.com/Article/details/gppmrhkaq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fktsv.cn/Article/details/goaxdbbtt.sHtML

[S24] C：获取本地时间
来源：http://mobile.yfazqb.com/Article/details/grwtlloxi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/gfabftqxy.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gygnunwuk.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gsrjqddlo.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/gukxbjcfq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.tarul.cn/Article/details/gbaeedbjx.sHtML

[S27] C：定义常量
来源：http://blog.bbcook.cn/Article/details/gdmkefhvs.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gwzvokqnp.sHtML

[S28] C：静态变量
来源：http://www.blog.vehdjk.com/Article/details/gyzqsdtrn.sHtML

static int counter = 0;
来源：http://www.m.share.fktsv.cn/Article/details/gmpgqddkr.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/gsmpxwyzq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.sjlbkw.cn/Article/details/gdhuxwcyu.sHtML

[S30] C：头文件保护
来源：http://wap.sjlbkw.cn/Article/details/gtaxsbaax.sHtML

#ifndef X_H
来源：http://blog.vehdjk.com/Article/details/gcmspkdnl.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gtvkstqoe.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/ghdfwjiup.sHtML

[S31] C++：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gwfwjfvxx.sHtML

#include <iostream>
来源：http://m.share.vehdjk.com/Article/details/giwmaaipl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.bbcook.cn/Article/details/gnthfudkq.sHtML

[S32] C++：字符串
来源：http://mobile.vehdjk.com/Article/details/gxkclowbo.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gtspnjnxl.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/gpqmijcwa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/ggnxrgvwd.sHtML

[S34] C++：遍历 vector
来源：http://baike.vehdjk.com/Article/details/gahjimcnm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/gjjotoqdj.sHtML


<!-- 参考信息 -->