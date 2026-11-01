代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gevigigyu.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/gvuoywvgw.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgzkurhb.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/gextnybqb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gngextihw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.yfazqb.com/Article/details/gjogsfixi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjinfutwi.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/gcpkhquxk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.bbcook.cn/Article/details/ggqnjpnir.sHtML

[Q58] 累计求和
来源：http://www.m.share.yfazqb.com/Article/details/gpmujnips.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/glyzapjvw.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/godyycito.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.tarul.cn/Article/details/gzuaerfrp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.yfazqb.com/Article/details/gdbfoqifi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.yfazqb.com/Article/details/gljpaifpy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/gipojkhkt.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gwejwwryk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gpdybrtvi.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/gundnlbik.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gopecocua.sHtML

[Q63] 开启事务
来源：http://m.share.fktsv.cn/Article/details/gwawxfngr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.yfazqb.com/Article/details/gvrongkci.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/gsgbvaoze.sHtML

COMMIT;
来源：http://www.m.share.fktsv.cn/Article/details/gfszjrnes.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/gibvbawfp.sHtML

ROLLBACK;
来源：http://www.share.epnwcf.com/Article/details/grdujsrhd.sHtML

[Q66] 行锁查询
来源：http://www.blog.bbcook.cn/Article/details/gzerkzfkf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.tarul.cn/Article/details/gnqahqmos.sHtML

[Q67] 设置隔离级别
来源：http://m.share.epnwcf.com/Article/details/glilddeue.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/goudcykoa.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gfwesqway.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/geixfedsz.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/ghojzlgcv.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/gwqkoawbp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gkghkzpvm.sHtML

[Q70] 更新统计信息
来源：http://3g.vehdjk.com/Article/details/gwvvwqhyf.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/gjqbprozb.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/gqpxghcey.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.vehdjk.com/Article/details/gonpeqbyu.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gymwbogne.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/gwmvvpwar.sHtML

[Q73] 查看表状态
来源：http://read.share.vehdjk.com/Article/details/gaokicfgh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gehgligjg.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/goudebpby.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gamnfewxz.sHtML

[Q75] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gzrueigeu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gsvgzojss.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.bbcook.cn/Article/details/gcyvhwclx.sHtML

[Q76] 按天统计
来源：http://baike.yfazqb.com/Article/details/gfgvapsky.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gfvlboiqy.sHtML

[Q77] 时间加减
来源：http://3g.sjlbkw.cn/Article/details/gbfqwlirc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.bbcook.cn/Article/details/ghgrxxwqp.sHtML

[Q78] 当前时间
来源：http://mobile.bbcook.cn/Article/details/gbtkfncwv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/gtjejtvpj.sHtML

[Q79] 字符串拼接
来源：http://baike.epnwcf.com/Article/details/godtuxnxe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/gexkfbxfk.sHtML

[Q80] 字符串截取
来源：http://www.share.sjlbkw.cn/Article/details/gjenwdtri.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.yfazqb.com/Article/details/grgwfxhpz.sHtML

[Q81] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/grocqrnoz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gnrjomroa.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/gzmphfwwp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gnfqxfzqd.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gchzdfmmi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gukshwasu.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.yfazqb.com/Article/details/ghbnttxrz.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gucbucvxy.sHtML

[Q85] 数值取整
来源：http://wap.yfazqb.com/Article/details/gxmbjugdf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.epnwcf.com/Article/details/gzvvgwmea.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.vehdjk.com/Article/details/gkwicxbak.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/gsihrbigs.sHtML

[Q87] JSON 字段做条件
来源：http://3g.bbcook.cn/Article/details/gimzlewsl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fktsv.cn/Article/details/guysdhqro.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fktsv.cn/Article/details/gftmchccl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gjzvwkkay.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gzddgachs.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gvfjusadd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/ginlbxefr.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/giuwsimre.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.epnwcf.com/Article/details/gmynfaxdj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwdiflahn.sHtML

R. Bash 专题
来源：http://www.blog.yfazqb.com/Article/details/ghovxvwin.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glhvsxrdr.sHtML

[R01] shebang 与严格模式
来源：http://baike.fktsv.cn/Article/details/ghucdixha.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fktsv.cn/Article/details/gzcyqtbxr.sHtML

set -euo pipefail
来源：http://blog.vehdjk.com/Article/details/gvyjceujx.sHtML

[R02] 变量赋值与使用
来源：http://3g.epnwcf.com/Article/details/gbhpcqdms.sHtML

name="Tom"; echo "$name"
来源：http://blog.sjlbkw.cn/Article/details/ghusflsko.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/gwprxmpep.sHtML

readonly PI=3.14
来源：http://www.m.share.vehdjk.com/Article/details/gsfxebloq.sHtML

[R04] 位置参数
来源：http://mobile.epnwcf.com/Article/details/gkiksunno.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fktsv.cn/Article/details/gfosrrqhy.sHtML

[R05] 参数默认值
来源：http://www.blog.bbcook.cn/Article/details/gttimrtao.sHtML

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/gcpfugcdk.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/gpsdacokt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/ghmqbljyt.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gfipyqqyy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gcaqsnlld.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/gqkkvigmp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/ghvzleeuc.sHtML

[R09] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gifkhcryj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/gmyeenrmo.sHtML

[R10] 正则匹配
来源：http://3g.bbcook.cn/Article/details/gxlkcwpia.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaugislv.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gqqrktxfk.sHtML

case "$1" in
来源：http://www.share.fktsv.cn/Article/details/gvwekjxio.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gvgugdxfv.sHtML

stop)  echo "停止" ;;
来源：http://read.share.yfazqb.com/Article/details/ghvofaqdg.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gfshuxkjb.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/gpianadjt.sHtML

[R12] for 遍历文件
来源：http://3g.vehdjk.com/Article/details/gqriotqpm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.vehdjk.com/Article/details/gswtxztna.sHtML

[R13] for 计数循环
来源：http://baike.tarul.cn/Article/details/ghujgmyao.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/geuiollbo.sHtML

[R14] C 风格 for
来源：http://wap.fktsv.cn/Article/details/grfrwbfwf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gkddokayh.sHtML

[R15] while 逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gfbjqnepq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.vehdjk.com/Article/details/gaiyofjqa.sHtML

[R16] until 等待条件
来源：http://blog.sjlbkw.cn/Article/details/gzfviqfyu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/gsmturulr.sHtML

[R17] 数组定义与取值
来源：http://m.share.tarul.cn/Article/details/gsujtezpb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/gvffpgogx.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gqrmsfukz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.yfazqb.com/Article/details/gqztkyzez.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gkfzjmler.sHtML

echo "${#arr[@]}"
来源：http://www.blog.bbcook.cn/Article/details/gzdqayghq.sHtML

[R20] 关联数组（字典）
来源：http://wap.sjlbkw.cn/Article/details/gndghiaqz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/ginlctqcc.sHtML

[R21] 字符串长度
来源：http://baike.yfazqb.com/Article/details/gyzvxexio.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/gqkktmxvg.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/glnbcmhte.sHtML

echo "${s:0:5}"
来源：http://www.m.share.sjlbkw.cn/Article/details/geldyival.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gdlupqqed.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.tarul.cn/Article/details/gwgthnrrr.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gyjuumwtv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/giegjyxhj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fktsv.cn/Article/details/gpzokfvaj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/gpejxslqw.sHtML

[R26] 命令替换
来源：http://www.share.yfazqb.com/Article/details/gunkvdfce.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/gnftxvoxy.sHtML

[R27] 算术展开
来源：http://www.share.epnwcf.com/Article/details/gwzrdnrkd.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/gxcmrzqmd.sHtML

[R28] 浮点运算
来源：http://read.share.bbcook.cn/Article/details/gtxtdmfvu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/ghftoejne.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gfswjiqoj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/gychrekcc.sHtML

[R30] 函数返回状态码
来源：http://www.share.tarul.cn/Article/details/gyelhdurs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/gwzizqfef.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/giyvsnznt.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.vehdjk.com/Article/details/gwohvhwjo.sHtML

[R32] 参数个数校验
来源：http://baike.fktsv.cn/Article/details/gwjitwvgp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gmkbfmfxo.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/gahiisayf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/gzmtkxuir.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/gskccorhh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gsnjihoge.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gqillvopi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/gxidcidss.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.sjlbkw.cn/Article/details/ghopvphqr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gndwobmwz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gpsnpjoeo.sHtML

files=$(ls -1)
来源：http://wap.epnwcf.com/Article/details/gyyupxnyj.sHtML

[R38] 管道串联
来源：http://mobile.sjlbkw.cn/Article/details/gwvcngdut.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.yfazqb.com/Article/details/gyvbgfevr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.tarul.cn/Article/details/gounhgcuu.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/gsovptiwu.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/gvhhhrric.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gkjymrqdo.sHtML

[R41] 丢弃输出
来源：http://read.share.vehdjk.com/Article/details/ghqapolfs.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gitedmxoq.sHtML

[R42] 输入重定向
来源：http://read.share.sjlbkw.cn/Article/details/glcqqykpv.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gfwldozld.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/gtjwhcpym.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gicwooeqe.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gzrpnplsp.sHtML

find . -mtime -7 -type f
来源：http://read.share.yfazqb.com/Article/details/gmnmnuaie.sHtML

[R45] 批量删除
来源：http://www.m.share.epnwcf.com/Article/details/geylzyovi.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/gusygawfe.sHtML

[R46] 递归替换文件内容
来源：http://baike.tarul.cn/Article/details/gocctqrgb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fktsv.cn/Article/details/gevuvqezk.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/guukpfkaa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fktsv.cn/Article/details/gyarcbart.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/grcnkzqel.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gxkbavgib.sHtML

[R49] awk 带条件
来源：http://mobile.tarul.cn/Article/details/gwpitulnv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.sjlbkw.cn/Article/details/gcozhgmpl.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/glxfverdi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/grzkrlfdm.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gccmrxlrh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.yfazqb.com/Article/details/gjeaygsvf.sHtML

[R52] 统计行数
来源：http://mobile.sjlbkw.cn/Article/details/gbazokjam.sHtML

wc -l a.txt
来源：http://m.share.fktsv.cn/Article/details/gsqgczfpn.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.yfazqb.com/Article/details/ginqibvdx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fktsv.cn/Article/details/gomiaymrp.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/ggogtqqbh.sHtML

diff a.txt b.txt
来源：http://www.m.share.bbcook.cn/Article/details/gmuiwxaiw.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/grumsnmbt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gmiwiwygr.sHtML

[R56] 远程拷贝
来源：http://www.blog.bbcook.cn/Article/details/ggwuzqemw.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/guybefzfl.sHtML

[R57] 远程执行命令
来源：http://www.share.bbcook.cn/Article/details/ghdhaqece.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gccznvxzl.sHtML

[R58] 下载文件
来源：http://wap.bbcook.cn/Article/details/gsqsprkls.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/gjizkakfy.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gsfnthnvb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.tarul.cn/Article/details/gypyyaxom.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gmdxeycbd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.tarul.cn/Article/details/gvpeddxsm.sHtML

[R61] 磁盘占用
来源：http://mobile.tarul.cn/Article/details/gmdpzhncu.sHtML

df -h;  du -sh *
来源：http://read.share.tarul.cn/Article/details/giwatmfad.sHtML

[R62] 找最占空间的文件
来源：http://3g.bbcook.cn/Article/details/geibjogwd.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/guvdiijms.sHtML

[R63] 内存与进程
来源：http://baike.bbcook.cn/Article/details/gdswlzjtf.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/glmkochlz.sHtML

[R64] 结束进程
来源：http://www.share.yfazqb.com/Article/details/gmftrbjcn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fktsv.cn/Article/details/goegfhxxx.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gciczgvtp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gwfknezoe.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/gaubivmyo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gttxxtbox.sHtML

[R67] 生成随机十六进制串
来源：http://3g.epnwcf.com/Article/details/gjejlcpto.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/gqpjrzwgk.sHtML

[R68] 计算文件校验值
来源：http://www.share.sjlbkw.cn/Article/details/gwpjthlne.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.bbcook.cn/Article/details/gcbuabtia.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gwknmvoez.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/guzodgctm.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/glkkwxtye.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gzulghfgi.sHtML

[R71] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gcvsjgoin.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.bbcook.cn/Article/details/ghpxdaneq.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.bbcook.cn/Article/details/ggwlepnjo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gwzuipffa.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gkiuvfkrq.sHtML

split -l 1000 big.log part_
来源：http://blog.vehdjk.com/Article/details/gfmghvyom.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gjggswefo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.bbcook.cn/Article/details/glprfpaxc.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gdwghkblx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/gnmlwrunh.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/gxtmnywsd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/grmdyvtqx.sHtML

[R77] 读取用户输入
来源：http://www.share.yfazqb.com/Article/details/gxiifcijr.sHtML

read -rp "请输入: " ans
来源：http://www.share.sjlbkw.cn/Article/details/gupmxascs.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/gnoxpwjjb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.epnwcf.com/Article/details/gcvjbnvpp.sHtML

[R79] 解析命令行选项
来源：http://wap.vehdjk.com/Article/details/gkyuxezuy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gvsvpcror.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/giailzhdy.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/ggwvmtren.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjetvfpmt.sHtML

S. C / C++ 专题
来源：http://www.m.share.tarul.cn/Article/details/gaakzxrbw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtejztbdz.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/grfnhbndc.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/gwpqtjlcc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gsdniousa.sHtML

[S02] C：变量与格式化输出
来源：http://blog.epnwcf.com/Article/details/gfqgephrv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/glgrpiwnp.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gnkvuusfh.sHtML

int x; scanf("%d", &x);
来源：http://3g.tarul.cn/Article/details/gnqgodzhw.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/gxpermjur.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gbsjpczkl.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/glakrqwft.sHtML

strlen(s)
来源：http://www.share.tarul.cn/Article/details/gvfmsqimw.sHtML

[S06] C：字符串比较
来源：http://www.share.epnwcf.com/Article/details/gfwwlrglz.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/gasdzxdql.sHtML

[S07] C：数组遍历求和
来源：http://mobile.bbcook.cn/Article/details/gdwartdic.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/gopakwrez.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/gfvkbarde.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.bbcook.cn/Article/details/gtdykgvgj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gluezkhub.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/gspxzaizl.sHtML

[S10] C：指针与解引用
来源：http://3g.epnwcf.com/Article/details/gupehtrum.sHtML

int *p = &a;  *p = 5;
来源：http://3g.yfazqb.com/Article/details/gywtogdkm.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gqlvjpndn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.vehdjk.com/Article/details/gpvymlxtt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.yfazqb.com/Article/details/gierrrwku.sHtML

fclose(f);
来源：http://3g.epnwcf.com/Article/details/guywwbveg.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/glmbicnrt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/gwhblfyjd.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gjfurpxzg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gesqrkecr.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gzxfwccsq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtnjhkai.sHtML

[S15] C：类型转换
来源：http://baike.bbcook.cn/Article/details/gljghkdvn.sHtML

(double) a / b
来源：http://baike.yfazqb.com/Article/details/gmctazkki.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gcyzqmyza.sHtML

x |= (1 << 3);
来源：http://wap.sjlbkw.cn/Article/details/gltvlcidd.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.epnwcf.com/Article/details/glernlchc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/grcrxzsje.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/gwxhkzflp.sHtML

int main(int argc, char **argv)
来源：http://wap.yfazqb.com/Article/details/gabahcyse.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/gymfijrpo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gffisqhmk.sHtML

[S20] C：二分查找
来源：http://baike.tarul.cn/Article/details/gyqyncaxp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gesvkzhrx.sHtML

[S21] C：字符类别判断
来源：http://baike.sjlbkw.cn/Article/details/ghefzyvce.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gnwrgmpgb.sHtML

[S22] C：字符串转数字
来源：http://mobile.tarul.cn/Article/details/gdrkrdteb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.vehdjk.com/Article/details/gxgojuctp.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/gurkwxdta.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.yfazqb.com/Article/details/gqfjayzcg.sHtML

[S24] C：获取本地时间
来源：http://blog.fktsv.cn/Article/details/gitphbpeo.sHtML


<!-- 参考信息 -->