代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://otr.guannengcc.top

[Q09] 创建唯一索引
来源：http://hmk.chenjidiqi.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://onl.yonumen.top

[Q10] 插入单行
来源：http://rkc.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wey.zdbjq.cn

[Q11] 一次插入多行
来源：http://iqu.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zsm.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://are.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vrh.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eff.xziqi.cn

[Q13] 忽略重复插入
来源：http://zll.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sds.xingfuxueyuan.xyz

[Q14] 存在则更新（upsert）
来源：http://iex.cdnleiting.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fjr.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mdy.yongpay.top

[Q15] 查询全部
来源：http://yod.hongshengwenyu.top

SELECT * FROM users;
来源：http://sgv.aizwys.cn

[Q16] 查询指定列
来源：http://eoe.jqgfzy.top

SELECT id, name FROM users;
来源：http://fpy.smart0.xyz

[Q17] 条件查询
来源：http://xin.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oou.shzxlz.cn

[Q18] 模糊匹配
来源：http://ofr.hesvh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vau.xuanzx.com

[Q19] 范围查询
来源：http://vsi.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://miu.yj20258888.top

[Q20] IN 列表
来源：http://ged.cdnleiting.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ems.cashguo.top

[Q21] 空值判断
来源：http://oxh.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ars.xingfuxueyuan.xyz

[Q22] 排序
来源：http://dft.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lds.yongpay.top

[Q23] 分页
来源：http://nho.tian-w.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tvr.yuanzhike.top

[Q24] 去重
来源：http://fcd.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://lby.tianlin.xyz

[Q25] 只取前 N 条
来源：http://wgt.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ddz.zdbjq.cn

[Q26] 计数
来源：http://pmz.zycfv.cn

SELECT COUNT(*) FROM users;
来源：http://sfp.yonumen.top

[Q27] 条件计数
来源：http://lpi.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://flz.yfazqb.com

[Q28] 求和与平均
来源：http://mbs.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zto.bbcook.cn

[Q29] 最大最小值
来源：http://kmz.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bdy.iojbl.cn

[Q30] 分组统计
来源：http://xoc.tanke756.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://axi.yj20258888.top

[Q31] 分组后过滤
来源：http://xsh.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aaa.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://vpk.jinghuilouyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mah.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ple.hongshengwenyu.top

[Q33] 多列分组
来源：http://ueo.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gqq.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://qgw.chenjidiqi.icu

SELECT * FROM (
来源：http://eyj.daxiang520.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bnk.birdmap.top

) t WHERE rn = 1;
来源：http://oza.c1oappe.top

[Q35] 内连接
来源：http://piz.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://orc.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://sre.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://alo.sysykeji.top

[Q37] 右连接
来源：http://jiw.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zka.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lrh.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sfi.nanxuanxn.top

[Q39] 自连接（查上下级）
来源：http://zqc.kuanghao11.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fym.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qvp.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bdt.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mzk.chenjidiqi.icu

[Q41] 多表连接
来源：http://rrs.52xcode.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ncr.xingfuxueyuan.xyz

JOIN users u ON u.id = o.user_id
来源：http://uvf.meibo888.top

JOIN products p ON p.id = o.product_id;
来源：http://hsc.uphjek.com

[Q42] 连接条件附加过滤
来源：http://pdl.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://vvi.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cbv.redwolf501.top

[Q43] 标量子查询
来源：http://pfk.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mql.vqdsnc.cn

[Q44] IN 子查询
来源：http://kve.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nxm.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://typ.hnxiangtu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aff.wangdashe.top

[Q46] NOT EXISTS 判断不存在
来源：http://gzw.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vov.zhijiandao.cn

[Q47] 与平均值比较
来源：http://xit.jiagoushi.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xfy.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://yqy.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wsy.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://rdy.yongpay.top

[Q49] 更新单行
来源：http://wws.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jlt.ehwqpu.com

[Q50] 批量更新
来源：http://svd.fengsongda.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ezi.zhongyouzk.top

[Q51] 用子查询更新
来源：http://yuw.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bvl.yj20258.top

[Q52] 删除指定行
来源：http://yfe.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://nzc.ybcxt.top

[Q53] 按条件删除
来源：http://knl.zhongyouzk.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aqp.feifeiyinyue.top

[Q54] 清空表
来源：http://tar.smart0.xyz

TRUNCATE TABLE logs;
来源：http://xaa.wangdashe.top

[Q55] 排名（并列占位）
来源：http://oko.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ehw.cashguo.top

[Q56] 密集排名（并列不占位）
来源：http://hpt.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vmc.jinyuanbaomall.cn

[Q57] 行号
来源：http://tnt.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lll.jiagoushi.top

[Q58] 累计求和
来源：http://kvb.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yhx.fzhhl.top

[Q59] 分组内累计
来源：http://bdg.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vnz.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://tjj.nanxuanxn.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kls.andypj.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wqm.gzhubu.top

[Q61] 移动平均
来源：http://iuz.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wsf.yonumen.top

[Q62] 分组占比
来源：http://lnd.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qfq.hywenlv.cn

[Q63] 开启事务
来源：http://vwz.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://slo.zhoulong.xyz

[Q64] 提交事务
来源：http://yis.zdbjq.cn

COMMIT;
来源：http://fwb.chenlongwang.top

[Q65] 回滚事务
来源：http://uka.chenzaomai.com

ROLLBACK;
来源：http://sxr.shzxlz.cn

[Q66] 行锁查询
来源：http://cio.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kqi.sufxvd.cn

[Q67] 设置隔离级别
来源：http://zkf.haohaochexian.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aio.0kj1m.cn

[Q68] 保存点
来源：http://vfl.birdmap.top

SAVEPOINT sp1;
来源：http://cgs.xylfe.cn

ROLLBACK TO sp1;
来源：http://svc.yvedp.cn

[Q69] 查看执行计划
来源：http://jnu.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zvo.0kj1m.cn

[Q70] 更新统计信息
来源：http://ifg.jqgfzy.top

ANALYZE TABLE users;
来源：http://cya.hysaishi.cn

[Q71] 查看建表语句
来源：http://qgx.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kon.hnqzz.top

[Q72] 查看索引
来源：http://iel.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://acq.hesvh.cn

[Q73] 查看表状态
来源：http://gtb.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dvx.hywenlv.cn

[Q74] 强制使用索引
来源：http://nii.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ivb.yfazqb.com

[Q75] 日期格式化
来源：http://ujq.hywenlv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aze.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lun.zhijiandao.cn

[Q76] 按天统计
来源：http://kyi.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yyz.shanyushiyangkeji.top

[Q77] 时间加减
来源：http://cfl.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ogt.jqgfzy.top

[Q78] 当前时间
来源：http://yxj.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kbo.sweek.top

[Q79] 字符串拼接
来源：http://eha.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mxn.xziqi.cn

[Q80] 字符串截取
来源：http://dhh.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zan.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://nvz.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jvy.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://tpd.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vym.redwolf501.top

[Q83] 大小写转换
来源：http://ccb.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vop.yanxiufei.cn

[Q84] 去除首尾空格
来源：http://cko.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://uhq.zhixingplan.top

[Q85] 数值取整
来源：http://ltq.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wsg.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://wri.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kxc.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://ejc.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ksc.ydzc1.top

[Q88] 行转列（条件聚合）
来源：http://tee.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uqy.kuanghao11.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nzm.aibaodan.cn

[Q89] 判断表是否存在
来源：http://gii.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cdr.chenzaomai.com

[Q90] 生成序号列
来源：http://zlw.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ags.zhiwuduotai.top

================================================================================
来源：http://qys.dashuyun.cn

R. Bash 专题
来源：http://jzv.tarul.cn

================================================================================
来源：http://xco.hfpthk.cn

[R01] shebang 与严格模式
来源：http://pcc.ybcxt.top

#!/usr/bin/env bash
来源：http://yfm.zhixingplan.top

set -euo pipefail
来源：http://khv.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://dcs.guowangkeji.top

name="Tom"; echo "$name"
来源：http://syk.tian-w.cn

[R03] 只读变量
来源：http://jvs.jqgfzy.top

readonly PI=3.14
来源：http://uzl.feifeiyinyue.top

[R04] 位置参数
来源：http://nge.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zls.guowangkeji.top

[R05] 参数默认值
来源：http://mud.fanxiaobao.xyz

name="${1:-default}"
来源：http://fgk.redwolf501.top

[R06] 判断命令是否存在
来源：http://sru.epnwcf.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uso.gaohongyu789.top

[R07] if 判断文件
来源：http://wbk.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cby.aibaodan.cn

[R08] 数值比较
来源：http://til.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sgc.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://lfo.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pvz.jyoumei.cn

[R10] 正则匹配
来源：http://oqs.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sud.fehbvm.com

[R11] case 多分支
来源：http://zut.yangfankeji.com

case "$1" in
来源：http://smk.jiagoushi.top

start) echo "启动" ;;
来源：http://nbd.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://sdw.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://smc.fzhhl.top

esac
来源：http://mns.chenzaomai.com

[R12] for 遍历文件
来源：http://elv.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://zuz.0kj1m.cn

[R13] for 计数循环
来源：http://ite.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://hck.svipenyu.cn

[R14] C 风格 for
来源：http://sjg.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xjf.chenzaomai.com

[R15] while 逐行读文件
来源：http://vqj.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ivc.ehwqpu.com

[R16] until 等待条件
来源：http://cwr.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iis.sysykeji.top

[R17] 数组定义与取值
来源：http://fxz.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hjp.quarkkingdee.top

[R18] 遍历数组
来源：http://zip.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lbx.yongpay.top

[R19] 数组长度
来源：http://bwk.yanxiufei.cn

echo "${#arr[@]}"
来源：http://hot.sufxvd.cn

[R20] 关联数组（字典）
来源：http://wxn.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://usi.shanyushiyangkeji.top

[R21] 字符串长度
来源：http://ghb.zhiwuduotai.top

echo "${#s}"
来源：http://adv.jinghuilouyu.cn

[R22] 截取子串
来源：http://drf.tianlin.xyz

echo "${s:0:5}"
来源：http://iwc.uphjek.com

[R23] 字符串替换
来源：http://piu.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rnn.shzxlz.cn

[R24] 大小写转换
来源：http://xyb.snrcjt.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uzu.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://bmq.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://iym.yanxiufei.cn

[R26] 命令替换
来源：http://dnh.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://oft.ivvv.top

[R27] 算术展开
来源：http://nfy.nwbrower.top

echo $((1 + 2 * 3))
来源：http://qxl.zhixingplan.top

[R28] 浮点运算
来源：http://rge.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://gzn.hnqzz.top

[R29] 定义函数
来源：http://rbh.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://trg.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://bvp.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://cqn.ybcxt.top

[R31] 局部变量
来源：http://zgm.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://rzg.sjlbkw.cn

[R32] 参数个数校验
来源：http://tsh.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tge.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://tkh.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yfa.wangdashe.top

[R34] 退出时清理
来源：http://kjo.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://zum.9152youxi.cn

[R35] 后台执行并等待
来源：http://acl.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://efc.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://pzs.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cpk.fengsongda.top

[R37] 把输出赋给变量
来源：http://qsh.kuanghao11.cn

files=$(ls -1)
来源：http://enj.gogol.net.cn

[R38] 管道串联
来源：http://twi.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://kpk.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://cra.aizwys.cn

cmd > out.log 2>&1
来源：http://pdf.guannengcc.top

[R40] 追加写日志
来源：http://wni.gaohongyu789.top

echo "log" >> out.log
来源：http://nrt.feifeiyinyue.top

[R41] 丢弃输出
来源：http://ysw.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://uld.cashguo.top

[R42] 输入重定向
来源：http://kbb.sxryk.cn

wc -l < a.txt
来源：http://ckr.yanxiufei.cn

[R43] 按名字查找文件
来源：http://svl.zhoulong.xyz

find . -name "*.log" -type f
来源：http://doe.316326.xyz

[R44] 按修改时间查找
来源：http://yic.zhixingplan.top

find . -mtime -7 -type f
来源：http://lvr.fengsongda.top

[R45] 批量删除
来源：http://fjv.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://owx.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://sxx.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xid.shuidangran.top

[R47] sed 单行替换
来源：http://iug.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://okk.xuanzx.com

[R48] awk 取指定列
来源：http://ifz.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://pgj.ybcxt.top

[R49] awk 带条件
来源：http://wco.hywenlv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wni.tianlin.xyz

[R50] awk 求和
来源：http://foi.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://oud.xylfe.cn

[R51] 排序去重取前几
来源：http://utr.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sma.yvedp.cn

[R52] 统计行数
来源：http://osw.birdmap.top

wc -l a.txt
来源：http://heo.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://rjp.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xyq.hongshengwenyu.top

[R54] 比较两个文件
来源：http://xxk.jqgfzy.top

diff a.txt b.txt
来源：http://ctb.zhixingplan.top

[R55] 压缩与解压
来源：http://duo.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mpy.aizwys.cn

[R56] 远程拷贝
来源：http://fsy.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://uit.snrcjt.cn

[R57] 远程执行命令
来源：http://yhb.gaohongyu789.top


<!-- 参考信息 -->