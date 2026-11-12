代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ynl.uphjek.com

[Q18] 模糊匹配
来源：http://tbt.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dzh.9152youxi.cn

[Q19] 范围查询
来源：http://ncs.tanke756.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kot.yvedp.cn

[Q20] IN 列表
来源：http://bmc.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mgr.nanxuanxn.top

[Q21] 空值判断
来源：http://pyd.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ejm.xuanzx.com

[Q22] 排序
来源：http://ozm.sufxvd.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bqg.xingfuxueyuan.xyz

[Q23] 分页
来源：http://asn.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://axq.zhoulong.xyz

[Q24] 去重
来源：http://bur.shanyushiyangtech.top

SELECT DISTINCT city FROM users;
来源：http://vrw.chenlongwang.top

[Q25] 只取前 N 条
来源：http://bsy.xylfe.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://asf.xinyue.icu

[Q26] 计数
来源：http://gdb.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://fvb.iojbl.cn

[Q27] 条件计数
来源：http://nxo.snrcjt.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hjb.zdbjq.cn

[Q28] 求和与平均
来源：http://mru.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mlx.yuxming.cn

[Q29] 最大最小值
来源：http://koy.dianchejie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hov.fktsv.cn

[Q30] 分组统计
来源：http://vfz.jiagoushi.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jxl.zdbjq.cn

[Q31] 分组后过滤
来源：http://zbj.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://erg.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://tuv.gzhubu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cwc.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yyo.jianghu66.top

[Q33] 多列分组
来源：http://ezo.316326.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rnf.yfazqb.com

[Q34] 每组取第一条
来源：http://dgw.hywenlv.cn

SELECT * FROM (
来源：http://kxe.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ftm.snrcjt.cn

) t WHERE rn = 1;
来源：http://vss.ppjwa.cn

[Q35] 内连接
来源：http://sur.dashuyun.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tgi.cqqwz.cn

[Q36] 左连接
来源：http://ggq.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cta.zhijiandao.cn

[Q37] 右连接
来源：http://ruj.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tww.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lnb.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ebd.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://gsi.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mzk.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yal.daria6918.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ujq.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://szg.c1oappe.top

[Q41] 多表连接
来源：http://otj.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://okk.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://upa.tianlin.xyz

JOIN products p ON p.id = o.product_id;
来源：http://edm.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://bwf.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://umw.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vjh.tanke756.top

[Q43] 标量子查询
来源：http://kcb.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xyx.sufxvd.cn

[Q44] IN 子查询
来源：http://pxp.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zlq.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://uls.meibo888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mzo.c1oappe.top

[Q46] NOT EXISTS 判断不存在
来源：http://ovj.jqgfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ppo.nanxuanxn.top

[Q47] 与平均值比较
来源：http://rra.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tsj.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://wqj.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://duz.guowangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://hhi.jinqigfzy.top

[Q49] 更新单行
来源：http://nze.nanxinkj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jil.uphjek.com

[Q50] 批量更新
来源：http://zrx.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qna.smart0.xyz

[Q51] 用子查询更新
来源：http://upw.nanxinkj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nyz.uphjek.com

[Q52] 删除指定行
来源：http://trf.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://akx.yj20258888.top

[Q53] 按条件删除
来源：http://gpe.birdmap.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://frp.hammf.cn

[Q54] 清空表
来源：http://bun.daria6918.cn

TRUNCATE TABLE logs;
来源：http://pho.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://iks.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jbv.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://nfu.jlsjyb.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dcb.zhengqikj.top

[Q57] 行号
来源：http://tfe.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ocy.quarkkingdee.top

[Q58] 累计求和
来源：http://lfv.sjlbkw.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nvw.yvedp.cn

[Q59] 分组内累计
来源：http://nbf.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xdx.c1oappe.top

[Q60] 取上一行 / 下一行
来源：http://wep.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jyu.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tfz.9152youxi.cn

[Q61] 移动平均
来源：http://oda.meibo888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qto.316326.xyz

[Q62] 分组占比
来源：http://ovj.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gvc.fktsv.cn

[Q63] 开启事务
来源：http://ghy.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bsp.havefunace.top

[Q64] 提交事务
来源：http://ibv.hnxiangtu.top

COMMIT;
来源：http://esq.yangfankeji.com

[Q65] 回滚事务
来源：http://dwk.shzxlz.cn

ROLLBACK;
来源：http://urw.yvedp.cn

[Q66] 行锁查询
来源：http://wsm.yonumen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://klg.fktsv.cn

[Q67] 设置隔离级别
来源：http://wao.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dcm.hcnkem.com

[Q68] 保存点
来源：http://vtz.havefunace.top

SAVEPOINT sp1;
来源：http://iay.bbcook.cn

ROLLBACK TO sp1;
来源：http://ctm.c1oappe.top

[Q69] 查看执行计划
来源：http://pqq.zhengqikj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ylu.fanxiaobao.xyz

[Q70] 更新统计信息
来源：http://onc.cheryme.top

ANALYZE TABLE users;
来源：http://xkw.hnxiangtu.top

[Q71] 查看建表语句
来源：http://los.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wcs.zhijiandao.cn

[Q72] 查看索引
来源：http://qxu.ydzc1.top

SHOW INDEX FROM users;
来源：http://mfe.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://mfo.chenlongwang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jws.bjfxy.top

[Q74] 强制使用索引
来源：http://rtv.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oeq.xuetiantiany.cn

[Q75] 日期格式化
来源：http://gwo.wangdashe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wnk.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://evu.havefunace.top

[Q76] 按天统计
来源：http://udm.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vsc.ybcxt.top

[Q77] 时间加减
来源：http://dlt.pycfn.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://smk.zhiwuduotai.top

[Q78] 当前时间
来源：http://kwz.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://amd.ppjwa.cn

[Q79] 字符串拼接
来源：http://rnw.yonumen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nrj.nanxinkj.top

[Q80] 字符串截取
来源：http://mol.wangdashe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qbj.zhaomingkeji.xyz

[Q81] 字符串替换
来源：http://ogm.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ozp.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://auf.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dxs.ybcxt.top

[Q83] 大小写转换
来源：http://wpj.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gwy.yonumen.top

[Q84] 去除首尾空格
来源：http://xng.cqqwz.cn

SELECT TRIM(name) FROM users;
来源：http://til.fengsongda.top

[Q85] 数值取整
来源：http://qji.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rmi.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://cye.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qhv.yj202588.top

[Q87] JSON 字段做条件
来源：http://tyi.chenjidiqi.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gcd.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://wdw.jyoumei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tdz.hysaishi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://upv.zhoulong.xyz

[Q89] 判断表是否存在
来源：http://flk.316326.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aiv.quarkkingdee.top

[Q90] 生成序号列
来源：http://amx.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wfn.nwbrower.top

================================================================================
来源：http://zpi.xuetiantiany.cn

R. Bash 专题
来源：http://loi.gogol.net.cn

================================================================================
来源：http://myi.yfazqb.com

[R01] shebang 与严格模式
来源：http://its.hywenlv.cn

#!/usr/bin/env bash
来源：http://nqu.guannengcc.top

set -euo pipefail
来源：http://qwa.daxiang520.top

[R02] 变量赋值与使用
来源：http://cwy.zdqjudy.top

name="Tom"; echo "$name"
来源：http://qpf.vqdsnc.cn

[R03] 只读变量
来源：http://lht.fanxiaobao.xyz

readonly PI=3.14
来源：http://asq.gotoacloud.top

[R04] 位置参数
来源：http://qxt.yj20258.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vym.vehdjk.com

[R05] 参数默认值
来源：http://qzh.snrcjt.cn

name="${1:-default}"
来源：http://gzn.xylfe.cn

[R06] 判断命令是否存在
来源：http://edw.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://edc.cucudq.cn

[R07] if 判断文件
来源：http://vmu.xinyue.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zyf.gotoacloud.top

[R08] 数值比较
来源：http://ksw.zhoulong.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://ein.shzxlz.cn

[R09] 字符串比较
来源：http://ppq.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lij.chenjidiqi.icu

[R10] 正则匹配
来源：http://zsg.smart0.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qyb.cheryme.top

[R11] case 多分支
来源：http://nua.jianghu66.top

case "$1" in
来源：http://yfr.iojbl.cn

start) echo "启动" ;;
来源：http://afo.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://doq.tanke756.top

*)     echo "未知命令" ;;
来源：http://bvi.xylfe.cn

esac
来源：http://bvx.gotoacloud.top

[R12] for 遍历文件
来源：http://urm.yonumen.top

for f in *.txt; do echo "$f"; done
来源：http://eqr.xuanzx.com

[R13] for 计数循环
来源：http://gxl.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://ffv.haohaochexian.top

[R14] C 风格 for
来源：http://ksq.wangdashe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iis.hnxiangtu.top

[R15] while 逐行读文件
来源：http://cej.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qap.daxiang520.top

[R16] until 等待条件
来源：http://kpi.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://htp.ywan-chungtsiang.top

[R17] 数组定义与取值
来源：http://pzx.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://lop.0kj1m.cn

[R18] 遍历数组
来源：http://gbj.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kga.jlsjyb.cn

[R19] 数组长度
来源：http://igy.yj20258.top

echo "${#arr[@]}"
来源：http://ejx.guowangkeji.top

[R20] 关联数组（字典）
来源：http://erp.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ypl.hnqzz.top

[R21] 字符串长度
来源：http://cig.vehdjk.com

echo "${#s}"
来源：http://lgj.daxiang520.top

[R22] 截取子串
来源：http://nou.jiagoushi.top

echo "${s:0:5}"
来源：http://mue.pengpengdd.cyou

[R23] 字符串替换
来源：http://buq.iojbl.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sjr.xziqi.cn

[R24] 大小写转换
来源：http://kah.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hcp.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://ajz.fengsongda.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zvf.yvedp.cn

[R26] 命令替换
来源：http://pgd.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://xfk.cqqwz.cn

[R27] 算术展开
来源：http://ysp.redwolf501.top

echo $((1 + 2 * 3))
来源：http://kqr.gaohongyu789.top

[R28] 浮点运算
来源：http://yvy.gaohongyu789.top

echo "scale=2; 10/3" | bc
来源：http://vda.bbcook.cn

[R29] 定义函数
来源：http://huh.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uok.iojbl.cn

[R30] 函数返回状态码
来源：http://qob.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://rgl.guowangkeji.top

[R31] 局部变量
来源：http://oye.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://yvf.daria6918.cn

[R32] 参数个数校验
来源：http://zum.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cop.cashguo.top

[R33] 捕获错误并提示行号
来源：http://qgb.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://byb.chenjidiqi.icu

[R34] 退出时清理
来源：http://qhq.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://ddf.fanxiaobao.xyz

[R35] 后台执行并等待
来源：http://qzn.wangdashe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pal.andypj.xyz

[R36] 并发执行多个任务
来源：http://tdq.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pix.ppjwa.cn

[R37] 把输出赋给变量
来源：http://qck.yueranfly.top

files=$(ls -1)
来源：http://fiq.hywenlv.cn

[R38] 管道串联
来源：http://pqu.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://rwi.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://lyf.dianchejie.cn

cmd > out.log 2>&1
来源：http://hsx.chenzaomai.com

[R40] 追加写日志
来源：http://xuz.redwolf501.top

echo "log" >> out.log
来源：http://gmf.9152youxi.cn

[R41] 丢弃输出
来源：http://suk.vehdjk.com

cmd >/dev/null 2>&1
来源：http://pwf.aizwys.cn

[R42] 输入重定向
来源：http://wuj.cheryme.top

wc -l < a.txt
来源：http://ota.gogol.net.cn

[R43] 按名字查找文件
来源：http://gjz.jinqigfzy.top

find . -name "*.log" -type f
来源：http://ykx.yj20258.top

[R44] 按修改时间查找
来源：http://kos.fehbvm.com

find . -mtime -7 -type f
来源：http://dzx.yonumen.top

[R45] 批量删除
来源：http://umz.c1oappe.top

find . -name "*.tmp" -delete
来源：http://uxz.yj202588.top

[R46] 递归替换文件内容
来源：http://iay.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fwh.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://cyy.zhaomingkeji.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://zoo.nwbrower.top

[R48] awk 取指定列
来源：http://zbr.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://cbt.nanxuanxn.top

[R49] awk 带条件
来源：http://kwe.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://heu.ybcxt.top

[R50] awk 求和
来源：http://rtg.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://wzb.fzhhl.top

[R51] 排序去重取前几
来源：http://ybh.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://uaw.xingfuxueyuan.xyz

[R52] 统计行数
来源：http://dzc.tianlin.xyz

wc -l a.txt
来源：http://jcg.uphjek.com

[R53] 查看文件头与实时尾
来源：http://rhq.svipenyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lkp.pengpengdd.cyou

[R54] 比较两个文件
来源：http://rbh.hysaishi.cn

diff a.txt b.txt
来源：http://nmk.vqdsnc.cn

[R55] 压缩与解压
来源：http://edf.iojbl.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wns.fengsongda.top

[R56] 远程拷贝
来源：http://ycv.pycfn.com

scp file user@host:/path/
来源：http://ged.yuanzhike.top

[R57] 远程执行命令
来源：http://jgq.cdnleiting.top

ssh user@host 'uptime'
来源：http://gwq.shanyushiyangkeji.top

[R58] 下载文件
来源：http://zmi.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gak.zhixingplan.top

[R59] 发 POST JSON
来源：http://aew.bjfxy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ldd.epnwcf.com

[R60] 只看 HTTP 状态码
来源：http://kli.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ntf.cheryme.top

[R61] 磁盘占用
来源：http://pao.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://lmj.epnwcf.com

[R62] 找最占空间的文件
来源：http://tvk.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://klc.sjlbkw.cn

[R63] 内存与进程
来源：http://rpq.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://ywu.hongshengwenyu.top

[R64] 结束进程
来源：http://jeu.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://ygi.cheryme.top

[R65] 查看端口占用
来源：http://eme.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mcm.yj20258888.top

[R66] 定时任务
来源：http://cfd.jiagoushi.top

crontab -e;  crontab -l
来源：http://lly.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://bix.svipenyu.cn


<!-- 参考信息 -->