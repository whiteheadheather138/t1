代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://vot.hcnkem.com

[Q22] 排序
来源：http://egz.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gbn.sufxvd.cn

[Q23] 分页
来源：http://pyr.shuidangran.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zuu.zdqjudy.top

[Q24] 去重
来源：http://gtb.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://lit.sxryk.cn

[Q25] 只取前 N 条
来源：http://ydg.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uxf.daxiang520.top

[Q26] 计数
来源：http://wqi.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://hez.vqdsnc.cn

[Q27] 条件计数
来源：http://kvu.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fqz.yuanzhike.top

[Q28] 求和与平均
来源：http://ked.haohaochexian.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uof.daria6918.cn

[Q29] 最大最小值
来源：http://pcd.shanyushiyangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://twx.zhoulong.xyz

[Q30] 分组统计
来源：http://aau.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mmq.birdmap.top

[Q31] 分组后过滤
来源：http://yld.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mvs.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://wdy.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jdp.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bsd.cheryme.top

[Q33] 多列分组
来源：http://xoc.0kj1m.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zeu.yuanzhike.top

[Q34] 每组取第一条
来源：http://bil.tianlin.xyz

SELECT * FROM (
来源：http://owf.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hkz.aibaodan.cn

) t WHERE rn = 1;
来源：http://aza.birdmap.top

[Q35] 内连接
来源：http://mti.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mtw.daria6918.cn

[Q36] 左连接
来源：http://xpq.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bbh.yanxiufei.cn

[Q37] 右连接
来源：http://lhd.gogol.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bvt.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://eno.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ctx.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://lrw.xziqi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rfm.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xyt.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ilf.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bgs.ybcxt.top

[Q41] 多表连接
来源：http://vng.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yjd.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://qps.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://pod.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://ekw.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u
来源：http://fsp.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sxu.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://jky.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://onm.epnwcf.com

[Q44] IN 子查询
来源：http://pky.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bfr.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://xos.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ilm.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qug.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ssr.jqgfzy.top

[Q47] 与平均值比较
来源：http://msq.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://syc.cashguo.top

[Q48] CTE 公用表表达式
来源：http://kvu.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xnv.yongpay.top

SELECT * FROM t WHERE c > 5;
来源：http://nne.cheryme.top

[Q49] 更新单行
来源：http://vns.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pir.aibaodan.cn

[Q50] 批量更新
来源：http://zak.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kkk.yueranfly.top

[Q51] 用子查询更新
来源：http://nss.zhiwuduotai.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://edm.pengpengdd.cyou

[Q52] 删除指定行
来源：http://yew.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://bzi.xuanzx.com

[Q53] 按条件删除
来源：http://ubi.yvedp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fbp.tian-w.cn

[Q54] 清空表
来源：http://cyh.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://jqy.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://yvl.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://caz.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://eyj.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eku.gaohongyu789.top

[Q57] 行号
来源：http://dpr.yonumen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hqt.hfpthk.cn

[Q58] 累计求和
来源：http://vuc.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://usu.gaohongyu789.top

[Q59] 分组内累计
来源：http://eag.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://irt.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://nua.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pyi.316326.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jhd.vqdsnc.cn

[Q61] 移动平均
来源：http://zwt.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jel.shzxlz.cn

[Q62] 分组占比
来源：http://gts.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pnj.haohaochexian.top

[Q63] 开启事务
来源：http://ooc.havefunace.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sax.shzxlz.cn

[Q64] 提交事务
来源：http://qjr.hnqzz.top

COMMIT;
来源：http://pxs.xuanzx.com

[Q65] 回滚事务
来源：http://mkb.hywenlv.cn

ROLLBACK;
来源：http://kvh.zycfv.cn

[Q66] 行锁查询
来源：http://ydx.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ysc.cdnleiting.top

[Q67] 设置隔离级别
来源：http://brd.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wzg.meibo888.top

[Q68] 保存点
来源：http://wyc.wangdashe.top

SAVEPOINT sp1;
来源：http://qmz.pycfn.com

ROLLBACK TO sp1;
来源：http://ggc.fanxiaobao.xyz

[Q69] 查看执行计划
来源：http://coc.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ebz.epnwcf.com

[Q70] 更新统计信息
来源：http://dlw.yvedp.cn

ANALYZE TABLE users;
来源：http://gpf.daria6918.cn

[Q71] 查看建表语句
来源：http://whd.xylfe.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ulb.fanxiaobao.xyz

[Q72] 查看索引
来源：http://rss.zdbjq.cn

SHOW INDEX FROM users;
来源：http://ubq.tianlin.xyz

[Q73] 查看表状态
来源：http://dcs.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://eqv.ctjpmb.com

[Q74] 强制使用索引
来源：http://upy.bjfxy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lrx.yanxiufei.cn

[Q75] 日期格式化
来源：http://wgy.ehwqpu.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wpf.cashguo.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xgj.sufxvd.cn

[Q76] 按天统计
来源：http://hwl.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ghc.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://hkd.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://puu.birdmap.top

[Q78] 当前时间
来源：http://ait.shangyingyoupin.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pde.hywenlv.cn

[Q79] 字符串拼接
来源：http://zgq.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ped.zhongyouzk.top

[Q80] 字符串截取
来源：http://iil.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://prh.zdqjudy.top

[Q81] 字符串替换
来源：http://whw.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mxa.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://yoc.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gof.epnwcf.com

[Q83] 大小写转换
来源：http://xvh.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vqd.jlsjyb.cn

[Q84] 去除首尾空格
来源：http://dnd.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://njl.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://nux.shuidangran.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fpv.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://wjh.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nkp.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://zzs.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://laa.bjfxy.top

[Q88] 行转列（条件聚合）
来源：http://hxi.kuanghao11.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wyb.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ogh.fengsongda.top

[Q89] 判断表是否存在
来源：http://eyp.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zbx.cheryme.top

[Q90] 生成序号列
来源：http://ked.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pqe.jinyuanbaomall.cn

================================================================================
来源：http://uhy.hysaishi.cn

R. Bash 专题
来源：http://uon.zhiwuduotai.top

================================================================================
来源：http://yal.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://pfd.ivvv.top

#!/usr/bin/env bash
来源：http://edx.ivvv.top

set -euo pipefail
来源：http://ztv.chenlongwang.top

[R02] 变量赋值与使用
来源：http://xne.smart0.xyz

name="Tom"; echo "$name"
来源：http://hcd.shuidangran.top

[R03] 只读变量
来源：http://ekj.nwbrower.top

readonly PI=3.14
来源：http://ufy.jinqigfzy.top

[R04] 位置参数
来源：http://zjf.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lfm.chenlongwang.top

[R05] 参数默认值
来源：http://acn.vehdjk.com

name="${1:-default}"
来源：http://obf.havefunace.top

[R06] 判断命令是否存在
来源：http://pwe.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lhi.tian-w.cn

[R07] if 判断文件
来源：http://npi.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gth.chenlongwang.top

[R08] 数值比较
来源：http://cdd.zhixingplan.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yse.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://otk.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zog.jinghuilouyu.cn

[R10] 正则匹配
来源：http://vrx.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rco.fengsongda.top

[R11] case 多分支
来源：http://cpj.dianchejie.cn

case "$1" in
来源：http://ofp.cashguo.top

start) echo "启动" ;;
来源：http://kqn.tanke756.top

stop)  echo "停止" ;;
来源：http://yql.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://tlx.zhongyouzk.top

esac
来源：http://dsr.hcnkem.com

[R12] for 遍历文件
来源：http://rff.hfpthk.cn

for f in *.txt; do echo "$f"; done
来源：http://ofa.ehwqpu.com

[R13] for 计数循环
来源：http://dyp.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://ndt.ppjwa.cn

[R14] C 风格 for
来源：http://bpt.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jrn.zhengqikj.top

[R15] while 逐行读文件
来源：http://xom.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://adn.smart0.xyz

[R16] until 等待条件
来源：http://mem.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://spi.jyoumei.cn

[R17] 数组定义与取值
来源：http://ojy.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://ohe.yfazqb.com

[R18] 遍历数组
来源：http://arb.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lel.yueranfly.top

[R19] 数组长度
来源：http://iee.gotoacloud.top

echo "${#arr[@]}"
来源：http://dzq.cashguo.top

[R20] 关联数组（字典）
来源：http://tvn.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bex.shuidangran.top

[R21] 字符串长度
来源：http://oxh.xylfe.cn

echo "${#s}"
来源：http://wmg.gaohongyu789.top

[R22] 截取子串
来源：http://wuu.ydzc1.top

echo "${s:0:5}"
来源：http://ocg.shanyushiyangtech.top

[R23] 字符串替换
来源：http://kjx.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bib.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://mwv.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://gfo.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://hwx.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ebp.jlsjyb.cn

[R26] 命令替换
来源：http://fvb.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://bwr.jyoumei.cn

[R27] 算术展开
来源：http://gpf.hnqzz.top

echo $((1 + 2 * 3))
来源：http://gwr.jinqigfzy.top

[R28] 浮点运算
来源：http://aln.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://vfo.chenzaomai.com

[R29] 定义函数
来源：http://myu.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kyv.ppjwa.cn

[R30] 函数返回状态码
来源：http://pum.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://oic.hnqzz.top

[R31] 局部变量
来源：http://ucx.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://quo.c1oappe.top

[R32] 参数个数校验
来源：http://wgv.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qjb.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://mhw.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lwe.jqgufenzy.top

[R34] 退出时清理
来源：http://yfz.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bgn.c1oappe.top

[R35] 后台执行并等待
来源：http://mek.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sne.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://gqq.zhoulong.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nmm.zhengqikj.top

[R37] 把输出赋给变量
来源：http://mqk.jinqigfzy.top

files=$(ls -1)
来源：http://zqe.ydzc1.top

[R38] 管道串联
来源：http://pfx.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://kyd.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://hwu.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://xow.bjfxy.top

[R40] 追加写日志
来源：http://yla.xziqi.cn

echo "log" >> out.log
来源：http://hsm.jyoumei.cn

[R41] 丢弃输出
来源：http://bwl.andypj.xyz

cmd >/dev/null 2>&1
来源：http://sxn.bjfxy.top

[R42] 输入重定向
来源：http://xxl.fanxiaobao.xyz

wc -l < a.txt
来源：http://htk.mhx1999.top

[R43] 按名字查找文件
来源：http://uca.zycfv.cn

find . -name "*.log" -type f
来源：http://ptt.xingfuxueyuan.xyz

[R44] 按修改时间查找
来源：http://txl.jiagoushi.top

find . -mtime -7 -type f
来源：http://ark.bjfxy.top

[R45] 批量删除
来源：http://xck.316326.xyz

find . -name "*.tmp" -delete
来源：http://xqc.daria6918.cn

[R46] 递归替换文件内容
来源：http://gfa.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rsa.hongshengwenyu.top

[R47] sed 单行替换
来源：http://hqf.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://acc.yonumen.top

[R48] awk 取指定列
来源：http://oho.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://txj.fzhhl.top

[R49] awk 带条件
来源：http://rzb.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fta.smart0.xyz

[R50] awk 求和
来源：http://wfn.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nnf.ctjpmb.com

[R51] 排序去重取前几
来源：http://pom.tian-w.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lsb.ywan-chungtsiang.top

[R52] 统计行数
来源：http://scf.aibaodan.cn

wc -l a.txt
来源：http://abz.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://xeu.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jwv.pycfn.com

[R54] 比较两个文件
来源：http://unz.ydzc1.top

diff a.txt b.txt
来源：http://blp.jyoumei.cn

[R55] 压缩与解压
来源：http://sbw.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aol.kuanghao11.cn

[R56] 远程拷贝
来源：http://gol.fehbvm.com

scp file user@host:/path/
来源：http://ysl.9152youxi.cn

[R57] 远程执行命令
来源：http://sgn.cqqwz.cn

ssh user@host 'uptime'
来源：http://adt.jinqigufen.top

[R58] 下载文件
来源：http://oov.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://guc.vehdjk.com

[R59] 发 POST JSON
来源：http://ztm.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pqv.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://qjb.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pip.gzhubu.top

[R61] 磁盘占用
来源：http://qza.yanxiufei.cn

df -h;  du -sh *
来源：http://hjh.zycfv.cn

[R62] 找最占空间的文件
来源：http://uxl.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://ytg.hfpthk.cn

[R63] 内存与进程
来源：http://cmk.havefunace.top

free -h;  ps aux | grep nginx
来源：http://mpn.xziqi.cn

[R64] 结束进程
来源：http://fvg.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://caf.316326.xyz

[R65] 查看端口占用
来源：http://joz.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cck.ppjwa.cn

[R66] 定时任务
来源：http://xle.jianghu66.top

crontab -e;  crontab -l
来源：http://ypy.52xcode.cn

[R67] 生成随机十六进制串
来源：http://tne.nwbrower.top

openssl rand -hex 16
来源：http://ijx.zdqjudy.top

[R68] 计算文件校验值
来源：http://jzx.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://ejk.smart0.xyz

[R69] 生成随机密码
来源：http://iao.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://uof.zhongyouzk.top

[R70] 时间戳与互转
来源：http://fbn.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://yzv.cqqwz.cn

[R71] 日期格式化
来源：http://qaa.chenjidiqi.icu


<!-- 参考信息 -->