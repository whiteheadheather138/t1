代发 wailian999

[Q63] 开启事务
来源：http://www.share.sjlbkw.cn/Article/details/gtpyiksjc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.epnwcf.com/Article/details/gyzcdemso.sHtML

[Q64] 提交事务
来源：http://read.share.sjlbkw.cn/Article/details/gavwxpldt.sHtML

COMMIT;
来源：http://mobile.sjlbkw.cn/Article/details/gwlokpauf.sHtML

[Q65] 回滚事务
来源：http://m.share.fktsv.cn/Article/details/gwaerannz.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/gntabnubn.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/glrfbnbnj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.tarul.cn/Article/details/gwlsahgoj.sHtML

[Q67] 设置隔离级别
来源：http://3g.vehdjk.com/Article/details/gywgsqrgm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.vehdjk.com/Article/details/gqbkkdefs.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gxlolocyd.sHtML

SAVEPOINT sp1;
来源：http://www.blog.epnwcf.com/Article/details/guiggifzt.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.bbcook.cn/Article/details/gtrgaievp.sHtML

[Q69] 查看执行计划
来源：http://3g.bbcook.cn/Article/details/gvtiirpnt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/gwibdtggn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.vehdjk.com/Article/details/gxwuacymb.sHtML

ANALYZE TABLE users;
来源：http://m.share.sjlbkw.cn/Article/details/glxkfkadm.sHtML

[Q71] 查看建表语句
来源：http://blog.sjlbkw.cn/Article/details/gioadfxii.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.yfazqb.com/Article/details/gpxlreyyp.sHtML

[Q72] 查看索引
来源：http://blog.fktsv.cn/Article/details/gmcgyblfd.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/grjirhcqy.sHtML

[Q73] 查看表状态
来源：http://blog.vehdjk.com/Article/details/gueyvrcah.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.vehdjk.com/Article/details/gwvocpgtk.sHtML

[Q74] 强制使用索引
来源：http://blog.sjlbkw.cn/Article/details/ggeaispsm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.vehdjk.com/Article/details/gipclkheh.sHtML

[Q75] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gtkfjznnk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.epnwcf.com/Article/details/gdkonhnwf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.yfazqb.com/Article/details/gfsrkvtll.sHtML

[Q76] 按天统计
来源：http://wap.sjlbkw.cn/Article/details/glrlkcqst.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.vehdjk.com/Article/details/gsixonfbz.sHtML

[Q77] 时间加减
来源：http://baike.bbcook.cn/Article/details/gqewtkqbg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.epnwcf.com/Article/details/gqaeixcpw.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/gsmvanawu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.yfazqb.com/Article/details/gcceoqvzj.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gkgavaxgy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/gccplhggu.sHtML

[Q80] 字符串截取
来源：http://read.share.vehdjk.com/Article/details/gqckzbjuj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fktsv.cn/Article/details/gdorrdabj.sHtML

[Q81] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrsehgqx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/geopzqlgg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fktsv.cn/Article/details/gmpixqwbg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gjjzvbtcj.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gtaikhnaf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gxjkqlxuj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.vehdjk.com/Article/details/gvzlchkzt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gvcyuttwb.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/gdhednqkb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/gukyfgifr.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gpdpttaxr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/grxveutfj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gffjqfhym.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.epnwcf.com/Article/details/gvifnrgol.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.yfazqb.com/Article/details/gdtcatdnl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.sjlbkw.cn/Article/details/gqcvozznb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.tarul.cn/Article/details/gcmusddoc.sHtML

[Q89] 判断表是否存在
来源：http://3g.sjlbkw.cn/Article/details/gxauhyqwb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.sjlbkw.cn/Article/details/gfndgwyuy.sHtML

[Q90] 生成序号列
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfdpqxct.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/gecfbbxls.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gvhcpmsmh.sHtML

R. Bash 专题
来源：http://www.m.share.vehdjk.com/Article/details/gwbujbrzw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyhdlpvbb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.tarul.cn/Article/details/gcrswlilf.sHtML

#!/usr/bin/env bash
来源：http://wap.fktsv.cn/Article/details/gveuhpsrt.sHtML

set -euo pipefail
来源：http://www.blog.fktsv.cn/Article/details/gadcwchzm.sHtML

[R02] 变量赋值与使用
来源：http://wap.bbcook.cn/Article/details/gtsnfjufr.sHtML

name="Tom"; echo "$name"
来源：http://www.share.epnwcf.com/Article/details/gnkcufjbs.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gqkzykjqk.sHtML

readonly PI=3.14
来源：http://www.share.fktsv.cn/Article/details/gtzqlqzcj.sHtML

[R04] 位置参数
来源：http://www.blog.tarul.cn/Article/details/goqsudncb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/gbfphxwlu.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/gsbbuspvy.sHtML

name="${1:-default}"
来源：http://www.m.share.tarul.cn/Article/details/gbnkvbnbp.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/grbcuoifx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gglgthggm.sHtML

[R07] if 判断文件
来源：http://3g.fktsv.cn/Article/details/gqmnwuvqe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fktsv.cn/Article/details/gklajqshf.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/guvlhvngo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.tarul.cn/Article/details/gdaueoozp.sHtML

[R09] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gmyzxfpno.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.tarul.cn/Article/details/gjhpqabda.sHtML

[R10] 正则匹配
来源：http://www.blog.epnwcf.com/Article/details/gxliwfvgw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.vehdjk.com/Article/details/gronvkrnk.sHtML

[R11] case 多分支
来源：http://www.blog.fktsv.cn/Article/details/gcpxyrxbh.sHtML

case "$1" in
来源：http://blog.tarul.cn/Article/details/grqgojfiu.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/glipfzcnc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.yfazqb.com/Article/details/ggxwgjpcf.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.bbcook.cn/Article/details/gerzrqjrp.sHtML

esac
来源：http://wap.bbcook.cn/Article/details/grhwemytn.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/goolrjwyn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gmoyttvyw.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gttyoydjc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsceklbl.sHtML

[R14] C 风格 for
来源：http://mobile.sjlbkw.cn/Article/details/gkqjzlqfk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/godrbvcwb.sHtML

[R15] while 逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gduxwauti.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/gbekkbrve.sHtML

[R16] until 等待条件
来源：http://www.blog.bbcook.cn/Article/details/gkbyiyrvx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gabylnkkz.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/gafgououi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fktsv.cn/Article/details/gnsdshrgg.sHtML

[R18] 遍历数组
来源：http://mobile.bbcook.cn/Article/details/gyhkggfqs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.epnwcf.com/Article/details/gzbohyvau.sHtML

[R19] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/goljfhisg.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/gixamffzg.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fktsv.cn/Article/details/gsczlwbky.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/guqbfewwi.sHtML

[R21] 字符串长度
来源：http://3g.fktsv.cn/Article/details/gdsdopqmq.sHtML

echo "${#s}"
来源：http://m.share.yfazqb.com/Article/details/gwkykdrmq.sHtML

[R22] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gyxytqnau.sHtML

echo "${s:0:5}"
来源：http://blog.tarul.cn/Article/details/gpxfvcqly.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gnlddvbjs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.tarul.cn/Article/details/gduocrahh.sHtML

[R24] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gizkgtqsj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.bbcook.cn/Article/details/gibhfkzji.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fktsv.cn/Article/details/glkqwuyqa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/ggriacmnh.sHtML

[R26] 命令替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwgkdklf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.epnwcf.com/Article/details/gtrdmmwof.sHtML

[R27] 算术展开
来源：http://www.m.share.sjlbkw.cn/Article/details/gihaacbyi.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gcafbjtnp.sHtML

[R28] 浮点运算
来源：http://m.share.tarul.cn/Article/details/gskvkxbdj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.yfazqb.com/Article/details/gmqaraazx.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gcoweevin.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gluvjiwud.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/ghykctwsn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gpviiyefk.sHtML

[R31] 局部变量
来源：http://blog.yfazqb.com/Article/details/godalctub.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fktsv.cn/Article/details/gruovtlac.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/gjhpsydot.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gvkuozbuu.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.epnwcf.com/Article/details/gzyknkyme.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmxeuknr.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/guafmbqhp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gdiyzonyd.sHtML

[R35] 后台执行并等待
来源：http://www.share.bbcook.cn/Article/details/gfwuufgnr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.vehdjk.com/Article/details/gapdrotkj.sHtML

[R36] 并发执行多个任务
来源：http://3g.sjlbkw.cn/Article/details/gkrkuwtuh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.yfazqb.com/Article/details/gdftsumny.sHtML

[R37] 把输出赋给变量
来源：http://baike.epnwcf.com/Article/details/gnleodcpa.sHtML

files=$(ls -1)
来源：http://read.share.tarul.cn/Article/details/gcfwvbttv.sHtML

[R38] 管道串联
来源：http://3g.fktsv.cn/Article/details/gdjbptetf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.yfazqb.com/Article/details/gzzujstmd.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.vehdjk.com/Article/details/goygsowkm.sHtML

cmd > out.log 2>&1
来源：http://m.share.epnwcf.com/Article/details/gjthlfzth.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gangdmood.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/gxtjaemdf.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/gomhwycav.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.tarul.cn/Article/details/grwxgafil.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/gnjgyxiij.sHtML

wc -l < a.txt
来源：http://www.blog.tarul.cn/Article/details/gtzypqyyv.sHtML

[R43] 按名字查找文件
来源：http://blog.bbcook.cn/Article/details/gfodeydog.sHtML

find . -name "*.log" -type f
来源：http://read.share.sjlbkw.cn/Article/details/gldeiviqx.sHtML

[R44] 按修改时间查找
来源：http://blog.yfazqb.com/Article/details/gkgfnjnds.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gbavxtcpy.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/gltendzdp.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.epnwcf.com/Article/details/ggzjtvwwn.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.tarul.cn/Article/details/gonlrjbyl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/gqzgiisuf.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/gqpaljoqh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gcqhicwxn.sHtML

[R48] awk 取指定列
来源：http://3g.epnwcf.com/Article/details/gfklloikr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gtsrfkbvx.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/gqlnorjuq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/gdjttoltv.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/guicelomu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/gwpukmmdf.sHtML

[R51] 排序去重取前几
来源：http://baike.sjlbkw.cn/Article/details/gegmlxgjv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/gzdrdnmcd.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gflumprjb.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gnkwszfbj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/gxfldybjn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/grnrquzox.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gubbnirlc.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/gyuyeaxuz.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/ggmyroext.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/gvqpttxjz.sHtML

[R56] 远程拷贝
来源：http://mobile.fktsv.cn/Article/details/gcuczwyah.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gdmyimjok.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gbxqgydia.sHtML

ssh user@host 'uptime'
来源：http://3g.fktsv.cn/Article/details/gnjgswhsu.sHtML

[R58] 下载文件
来源：http://www.blog.yfazqb.com/Article/details/gasodjxwy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gtgmgruyw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gopqtrujs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/gqbhnkemk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gqkjyxpvd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/ghcamvwnq.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/gryacckze.sHtML

df -h;  du -sh *
来源：http://www.share.vehdjk.com/Article/details/gudumskvl.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gbensbpwc.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/gsgmxotmd.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/gvlntwkmn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.tarul.cn/Article/details/gszfrxuhg.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gazryzqao.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/grzgfbaqt.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/geyjwjtig.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.bbcook.cn/Article/details/glkqhpmgw.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/gikevgxau.sHtML

crontab -e;  crontab -l
来源：http://m.share.yfazqb.com/Article/details/gzkkofxcv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gtlpnllgc.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/gzwqvijiq.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gyofdmtgx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fktsv.cn/Article/details/ginyhrfhr.sHtML

[R69] 生成随机密码
来源：http://3g.yfazqb.com/Article/details/gymriozci.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/gryexvtdu.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/goulqwfdy.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.epnwcf.com/Article/details/gxofrcoux.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gkqsvuzdm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fktsv.cn/Article/details/gvbxsrkkc.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/gfsbkxnpw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gxczhettx.sHtML

[R73] 分割大日志
来源：http://blog.sjlbkw.cn/Article/details/gaiicashs.sHtML

split -l 1000 big.log part_
来源：http://baike.yfazqb.com/Article/details/gqzurogyf.sHtML

[R74] 批量重命名
来源：http://www.m.share.fktsv.cn/Article/details/gfogbarpl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gtmpqpqha.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gjionbfha.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.vehdjk.com/Article/details/gzowuxwkl.sHtML

[R76] 使用临时文件
来源：http://baike.bbcook.cn/Article/details/gcykzyvim.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/golepsbjd.sHtML

[R77] 读取用户输入
来源：http://blog.tarul.cn/Article/details/gjckmkqcw.sHtML

read -rp "请输入: " ans
来源：http://www.share.sjlbkw.cn/Article/details/gfmcfezat.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/gywakldnj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.tarul.cn/Article/details/gwkipvnea.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.vehdjk.com/Article/details/gydmvnlid.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/ggpedrvlo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.vehdjk.com/Article/details/grctvfwhp.sHtML

time ./run.sh
来源：http://baike.yfazqb.com/Article/details/gizkoujqe.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbknzyetl.sHtML

S. C / C++ 专题
来源：http://www.share.epnwcf.com/Article/details/gxnxytutc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gehkloxds.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gxnrkjipj.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/gtzaafncb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/gfukgqhjt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gektbwcoq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gwcybgthk.sHtML

[S03] C：读入整数
来源：http://baike.yfazqb.com/Article/details/gucspeoqd.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/gbtdowpux.sHtML

[S04] C：字符串复制
来源：http://www.blog.tarul.cn/Article/details/gjninwvmq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/gqxhsobwn.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gkizzfczo.sHtML

strlen(s)
来源：http://www.blog.vehdjk.com/Article/details/gqupwuffb.sHtML

[S06] C：字符串比较
来源：http://www.share.bbcook.cn/Article/details/gzdnctduw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/ggamasbcw.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/glbnucqgb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/gclylbthp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gphckajvp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.bbcook.cn/Article/details/gcnertajk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/gflcqsnzi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fktsv.cn/Article/details/grwjvtygp.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/gkmcutqfm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.bbcook.cn/Article/details/gkortjplp.sHtML

[S11] C：逐行读文件
来源：http://baike.tarul.cn/Article/details/guxjlplxm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.vehdjk.com/Article/details/gmcsuqvfj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gyjplwdyj.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/ggwkakljd.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/gwtweuhqm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gcurmvexb.sHtML

[S13] C：宏定义
来源：http://read.share.tarul.cn/Article/details/gxtkyvawq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.tarul.cn/Article/details/giyeqlzhm.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/geoliiedp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/gqqwnjqbc.sHtML

[S15] C：类型转换
来源：http://read.share.tarul.cn/Article/details/gthhbxeoi.sHtML

(double) a / b
来源：http://blog.vehdjk.com/Article/details/gvncuqojs.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gocpxgwwe.sHtML

x |= (1 << 3);
来源：http://blog.tarul.cn/Article/details/gzgnbabij.sHtML

[S17] C：安全拼接字符串
来源：http://wap.tarul.cn/Article/details/gdbmpssrz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/gqritbyvq.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gpytjashe.sHtML

int main(int argc, char **argv)
来源：http://www.share.fktsv.cn/Article/details/gmprwxqdb.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/gdadlifmt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gohxljkbx.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gatrhoddj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gernlclgu.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/gchyuizex.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/geymnozbb.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gtcunqctk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gbpmcnlud.sHtML

[S23] C：随机数
来源：http://wap.yfazqb.com/Article/details/gttukzoke.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/gwkxkixsq.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/gfbtjewzx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.yfazqb.com/Article/details/gsjmkzrjt.sHtML

[S25] C：内存拷贝
来源：http://baike.bbcook.cn/Article/details/gjajjwmbh.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gshzczfrr.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/gtascldjj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.vehdjk.com/Article/details/grnhwecjv.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gifbgwqdw.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/ghrjacvhn.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/gbnnqoqhg.sHtML

static int counter = 0;
来源：http://www.share.vehdjk.com/Article/details/gtdxessca.sHtML

[S29] C：变参函数
来源：http://www.m.share.fktsv.cn/Article/details/giejfthtd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/ggdagahaa.sHtML

[S30] C：头文件保护
来源：http://www.blog.epnwcf.com/Article/details/ghfjyqgou.sHtML

#ifndef X_H
来源：http://www.share.sjlbkw.cn/Article/details/glmvzrkoz.sHtML

#define X_H
来源：http://mobile.fktsv.cn/Article/details/gbrnfrkzq.sHtML

#endif
来源：http://mobile.sjlbkw.cn/Article/details/gtaloflsz.sHtML

[S31] C++：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gtsvxtxoa.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/gtwywygvh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.epnwcf.com/Article/details/gajnlkhde.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/glulxsznx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gqjsbgquj.sHtML


<!-- 参考信息 -->