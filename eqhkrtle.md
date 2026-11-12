代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ekd.uphjek.com

[Q05] 重命名列
来源：http://pwu.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cvx.sufxvd.cn

[Q06] 删除列
来源：http://lgg.fktsv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yir.chenjidiqi.icu

[Q07] 删除表
来源：http://mxg.cucudq.cn

DROP TABLE IF EXISTS orders;
来源：http://pnw.gogol.net.cn

[Q08] 创建普通索引
来源：http://qnq.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uta.ppjwa.cn

[Q09] 创建唯一索引
来源：http://qby.xinyue.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gtg.dashuyun.cn

[Q10] 插入单行
来源：http://hhk.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cqz.daxiang520.top

[Q11] 一次插入多行
来源：http://irv.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://met.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://qtw.yvedp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ekn.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pgm.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://cam.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://slk.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://ygk.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ktu.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zft.pycfn.com

[Q15] 查询全部
来源：http://mfi.iojbl.cn

SELECT * FROM users;
来源：http://qhw.andypj.xyz

[Q16] 查询指定列
来源：http://bxf.cqqwz.cn

SELECT id, name FROM users;
来源：http://cgl.sweek.top

[Q17] 条件查询
来源：http://uji.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mxc.yonumen.top

[Q18] 模糊匹配
来源：http://wld.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://swp.jinqigfzy.top

[Q19] 范围查询
来源：http://zep.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vhu.jqgfzy.top

[Q20] IN 列表
来源：http://amw.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iwt.gaohongyu789.top

[Q21] 空值判断
来源：http://pmf.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mrp.jinyuanbaomall.cn

[Q22] 排序
来源：http://vdq.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jye.hesvh.cn

[Q23] 分页
来源：http://sbx.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qxd.hnxiangtu.top

[Q24] 去重
来源：http://ext.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://pob.tanke756.top

[Q25] 只取前 N 条
来源：http://ywl.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jti.jiagoushi.top

[Q26] 计数
来源：http://tgy.cheryme.top

SELECT COUNT(*) FROM users;
来源：http://crk.xinyue.icu

[Q27] 条件计数
来源：http://mjl.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iun.zhiwuduotai.top

[Q28] 求和与平均
来源：http://icl.bbcook.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fix.cashguo.top

[Q29] 最大最小值
来源：http://txh.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hju.yonumen.top

[Q30] 分组统计
来源：http://wjx.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yqv.cheryme.top

[Q31] 分组后过滤
来源：http://iwi.yvedp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qcr.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://ahw.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zro.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jtf.sufxvd.cn

[Q33] 多列分组
来源：http://wda.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rue.sjlbkw.cn

[Q34] 每组取第一条
来源：http://vyb.bjfxy.top

SELECT * FROM (
来源：http://gdf.yuxming.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qxc.316326.xyz

) t WHERE rn = 1;
来源：http://pfi.jqgfzy.top

[Q35] 内连接
来源：http://iki.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://abz.hnqzz.top

[Q36] 左连接
来源：http://fgp.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://phc.jiagoushi.top

[Q37] 右连接
来源：http://qkp.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hym.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://awc.jqgfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pmx.nwbrower.top

[Q39] 自连接（查上下级）
来源：http://qmi.sufxvd.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fjq.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ksk.zhoulong.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://kjk.ivvv.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ipc.yuanzhike.top

[Q41] 多表连接
来源：http://woc.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wiw.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://qft.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://qhb.cashguo.top

[Q42] 连接条件附加过滤
来源：http://llu.zhijiandao.cn

SELECT u.name, o.amount FROM users u
来源：http://fsd.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fuo.pengpengdd.cyou

[Q43] 标量子查询
来源：http://gni.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zvp.cdnleiting.top

[Q44] IN 子查询
来源：http://xem.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://izq.aibaodan.cn

[Q45] EXISTS 判断存在
来源：http://lrd.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://flq.shanyushiyangtech.top

[Q46] NOT EXISTS 判断不存在
来源：http://ydn.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://soo.gogol.net.cn

[Q47] 与平均值比较
来源：http://lit.jiagoushi.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qjk.bbcook.cn

[Q48] CTE 公用表表达式
来源：http://acj.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vkl.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://ogf.jqgufenzy.top

[Q49] 更新单行
来源：http://bzm.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hcj.cheryme.top

[Q50] 批量更新
来源：http://ked.fengsongda.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hcx.316326.xyz

[Q51] 用子查询更新
来源：http://qeo.yfazqb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://itb.cashguo.top

[Q52] 删除指定行
来源：http://rrn.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://ora.fzhhl.top

[Q53] 按条件删除
来源：http://exs.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ive.haohaochexian.top

[Q54] 清空表
来源：http://hgk.uphjek.com

TRUNCATE TABLE logs;
来源：http://qba.xuanzx.com

[Q55] 排名（并列占位）
来源：http://szt.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pod.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://byt.tian-w.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pul.guowangkeji.top

[Q57] 行号
来源：http://asf.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qwh.yj202588.top

[Q58] 累计求和
来源：http://ffx.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://djx.0kj1m.cn

[Q59] 分组内累计
来源：http://yyy.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mzd.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://umc.guowangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ymi.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xuk.vqdsnc.cn

[Q61] 移动平均
来源：http://iqq.hywenlv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jym.cheryme.top

[Q62] 分组占比
来源：http://kfz.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vog.vehdjk.com

[Q63] 开启事务
来源：http://gqc.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://oyv.xylfe.cn

[Q64] 提交事务
来源：http://cwb.jlsjyb.cn

COMMIT;
来源：http://kyx.vqdsnc.cn

[Q65] 回滚事务
来源：http://fma.fengsongda.top

ROLLBACK;
来源：http://frm.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://skd.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bkr.zdbjq.cn

[Q67] 设置隔离级别
来源：http://ubf.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://syn.meibo888.top

[Q68] 保存点
来源：http://zjr.hfpthk.cn

SAVEPOINT sp1;
来源：http://jeo.gzhubu.top

ROLLBACK TO sp1;
来源：http://oju.sxryk.cn

[Q69] 查看执行计划
来源：http://hdk.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rqk.sysykeji.top

[Q70] 更新统计信息
来源：http://fsn.jlsjyb.cn

ANALYZE TABLE users;
来源：http://gxh.nanxuanxn.top

[Q71] 查看建表语句
来源：http://weq.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uzg.havefunace.top

[Q72] 查看索引
来源：http://odd.zdbjq.cn

SHOW INDEX FROM users;
来源：http://rsp.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://blk.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vai.xziqi.cn

[Q74] 强制使用索引
来源：http://zoc.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uzf.ppjwa.cn

[Q75] 日期格式化
来源：http://ipz.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wud.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rus.jyoumei.cn

[Q76] 按天统计
来源：http://ywx.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://een.fehbvm.com

[Q77] 时间加减
来源：http://cbn.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nwr.yj20258888.top

[Q78] 当前时间
来源：http://lkv.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yrg.ehwqpu.com

[Q79] 字符串拼接
来源：http://meb.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bgb.ppjwa.cn

[Q80] 字符串截取
来源：http://fwe.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rnr.zhixingplan.top

[Q81] 字符串替换
来源：http://dab.fktsv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rft.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://cdj.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gdz.yangfankeji.com

[Q83] 大小写转换
来源：http://oqu.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uxx.yvedp.cn

[Q84] 去除首尾空格
来源：http://zzw.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://fca.sufxvd.cn

[Q85] 数值取整
来源：http://gpp.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zaq.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://jan.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://abk.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://ozo.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rtb.tian-w.cn

[Q88] 行转列（条件聚合）
来源：http://wsi.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yum.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qia.yuxming.cn

[Q89] 判断表是否存在
来源：http://sug.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ecb.nanxuanxn.top

[Q90] 生成序号列
来源：http://dxp.yongpay.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dmq.chenzaomai.com

================================================================================
来源：http://sgh.fzhhl.top

R. Bash 专题
来源：http://bgj.cqqwz.cn

================================================================================
来源：http://rrm.cdnleiting.top

[R01] shebang 与严格模式
来源：http://rjr.ppjwa.cn

#!/usr/bin/env bash
来源：http://yba.quarkkingdee.top

set -euo pipefail
来源：http://cgh.chenlongwang.top

[R02] 变量赋值与使用
来源：http://ydj.yangfankeji.com

name="Tom"; echo "$name"
来源：http://czw.hesvh.cn

[R03] 只读变量
来源：http://lms.yvedp.cn

readonly PI=3.14
来源：http://eom.zhixingplan.top

[R04] 位置参数
来源：http://qxa.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ifw.cucudq.cn

[R05] 参数默认值
来源：http://qkc.jyoumei.cn

name="${1:-default}"
来源：http://xqz.pycfn.com

[R06] 判断命令是否存在
来源：http://nom.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yre.hnqzz.top

[R07] if 判断文件
来源：http://vdt.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iwi.yonumen.top

[R08] 数值比较
来源：http://ucl.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qpt.uphjek.com

[R09] 字符串比较
来源：http://cpz.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oft.fengsongda.top

[R10] 正则匹配
来源：http://ukw.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nrp.quarkkingdee.top

[R11] case 多分支
来源：http://lxw.ybcxt.top

case "$1" in
来源：http://aas.meibo888.top

start) echo "启动" ;;
来源：http://bwh.aizwys.cn

stop)  echo "停止" ;;
来源：http://cvf.tian-w.cn

*)     echo "未知命令" ;;
来源：http://zzs.chenjidiqi.icu

esac
来源：http://cya.yfazqb.com

[R12] for 遍历文件
来源：http://oey.zhiwuduotai.top

for f in *.txt; do echo "$f"; done
来源：http://wxy.gotoacloud.top

[R13] for 计数循环
来源：http://tmv.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://yec.cucudq.cn

[R14] C 风格 for
来源：http://obd.ydjk.org.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wza.hysaishi.cn

[R15] while 逐行读文件
来源：http://qfy.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nrx.yfazqb.com

[R16] until 等待条件
来源：http://niq.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ked.tanke756.top

[R17] 数组定义与取值
来源：http://kdy.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://aqu.zhongyouzk.top

[R18] 遍历数组
来源：http://bgs.havefunace.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vdh.kuanghao11.cn

[R19] 数组长度
来源：http://uka.zhijiandao.cn

echo "${#arr[@]}"
来源：http://xrt.jianghu66.top

[R20] 关联数组（字典）
来源：http://lgj.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bys.hcnkem.com

[R21] 字符串长度
来源：http://rcz.xuetiantiany.cn

echo "${#s}"
来源：http://ygs.shangyingyoupin.top

[R22] 截取子串
来源：http://rwb.zhongyouzk.top

echo "${s:0:5}"
来源：http://uxz.kuanghao11.cn

[R23] 字符串替换
来源：http://cam.hammf.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fgg.zdqjudy.top

[R24] 大小写转换
来源：http://vox.yangfankeji.com

echo "${s^^}"; echo "${s,,}"
来源：http://kgl.jqgufenzy.top

[R25] 去后缀 / 去前缀
来源：http://cww.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kbm.ppjwa.cn

[R26] 命令替换
来源：http://yef.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://nup.jinyuanbaomall.cn

[R27] 算术展开
来源：http://jbf.pycfn.com

echo $((1 + 2 * 3))
来源：http://xgc.xziqi.cn

[R28] 浮点运算
来源：http://aqm.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://yzd.haohaochexian.top

[R29] 定义函数
来源：http://tyv.gaohongyu789.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fja.vehdjk.com

[R30] 函数返回状态码
来源：http://vri.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://dyt.0kj1m.cn

[R31] 局部变量
来源：http://eyx.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://lis.uphjek.com

[R32] 参数个数校验
来源：http://pph.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fyo.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://ogg.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ovi.yuanzhike.top

[R34] 退出时清理
来源：http://tqh.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://dip.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://twl.yj202588.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fgn.fzhhl.top

[R36] 并发执行多个任务
来源：http://xmr.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://emm.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://adf.jlsjyb.cn

files=$(ls -1)
来源：http://eys.wangdashe.top

[R38] 管道串联
来源：http://rid.yvedp.cn

cat a.txt | grep -i error | wc -l
来源：http://six.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://ndj.cucudq.cn

cmd > out.log 2>&1
来源：http://lhs.guowangkeji.top

[R40] 追加写日志
来源：http://rcw.yj202588.top

echo "log" >> out.log
来源：http://qeg.zhongyouzk.top

[R41] 丢弃输出
来源：http://vit.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://fjw.cashguo.top

[R42] 输入重定向
来源：http://hqs.pengpengdd.cyou

wc -l < a.txt
来源：http://til.fengsongda.top

[R43] 按名字查找文件
来源：http://unc.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://fse.aibaodan.cn

[R44] 按修改时间查找
来源：http://qla.haohaochexian.top

find . -mtime -7 -type f
来源：http://ook.jinyuanbaomall.cn

[R45] 批量删除
来源：http://sei.fktsv.cn

find . -name "*.tmp" -delete
来源：http://qwg.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://yyw.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rot.zhiwuduotai.top

[R47] sed 单行替换
来源：http://cht.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://low.yvedp.cn

[R48] awk 取指定列
来源：http://rox.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://kgc.zhengqikj.top

[R49] awk 带条件
来源：http://igg.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lgc.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://xno.uphjek.com

awk '{s += $2} END {print s}' a.txt
来源：http://lob.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://csn.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pld.yuanzhike.top

[R52] 统计行数
来源：http://hvw.dianchejie.cn

wc -l a.txt
来源：http://zjd.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://oby.xuanzx.com


<!-- 参考信息 -->