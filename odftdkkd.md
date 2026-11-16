代发 wailian999

);
来源：http://pxy.jqgufenzy.top

[Q03] 增加列
来源：http://wcu.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qem.aibaodan.cn

[Q04] 修改列类型
来源：http://ldt.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wvs.yj20258888.top

[Q05] 重命名列
来源：http://fsr.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jcb.gzhubu.top

[Q06] 删除列
来源：http://wbc.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://ags.jinqigfzy.top

[Q07] 删除表
来源：http://nvq.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://uep.snrcjt.cn

[Q08] 创建普通索引
来源：http://zyo.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://alp.zycfv.cn

[Q09] 创建唯一索引
来源：http://rou.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lqn.hammf.cn

[Q10] 插入单行
来源：http://omd.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://weg.fanxiaobao.xyz

[Q11] 一次插入多行
来源：http://xcm.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cek.shuidangran.top

[Q12] 插入后取自增 ID
来源：http://uja.hnxiangtu.top

INSERT INTO users (name) VALUES ('C');
来源：http://gjc.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ezy.nanxinkj.top

[Q13] 忽略重复插入
来源：http://bgf.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gua.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://nnm.yj20258888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dso.sxryk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://utm.zhongyouzk.top

[Q15] 查询全部
来源：http://mtf.yueranfly.top

SELECT * FROM users;
来源：http://dyf.guannengcc.top

[Q16] 查询指定列
来源：http://fdt.gzhubu.top

SELECT id, name FROM users;
来源：http://pik.guannengcc.top

[Q17] 条件查询
来源：http://fxx.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zkw.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://jra.tarul.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fkj.feifeiyinyue.top

[Q19] 范围查询
来源：http://irb.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ufm.hongshengwenyu.top

[Q20] IN 列表
来源：http://cie.jinqigufen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mwt.dianchejie.cn

[Q21] 空值判断
来源：http://zei.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://voq.quarkkingdee.top

[Q22] 排序
来源：http://bfw.ydjk.org.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xdc.cheryme.top

[Q23] 分页
来源：http://eor.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nui.yj20258.top

[Q24] 去重
来源：http://bqt.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://kag.sysykeji.top

[Q25] 只取前 N 条
来源：http://vni.xingfuxueyuan.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pxf.guowangkeji.top

[Q26] 计数
来源：http://dxg.ywan-chungtsiang.top

SELECT COUNT(*) FROM users;
来源：http://qka.gotoacloud.top

[Q27] 条件计数
来源：http://gjv.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://smw.andypj.xyz

[Q28] 求和与平均
来源：http://tkv.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jdi.haohaochexian.top

[Q29] 最大最小值
来源：http://cfs.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mom.nanxinkj.top

[Q30] 分组统计
来源：http://yhj.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ekv.dashuyun.cn

[Q31] 分组后过滤
来源：http://evt.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yjx.shuidangran.top

[Q32] 分组拼接字符串
来源：http://yth.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dav.52xcode.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hpe.andypj.xyz

[Q33] 多列分组
来源：http://ohi.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://owp.jyoumei.cn

[Q34] 每组取第一条
来源：http://ins.ppjwa.cn

SELECT * FROM (
来源：http://fok.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://env.316326.xyz

) t WHERE rn = 1;
来源：http://ysc.vehdjk.com

[Q35] 内连接
来源：http://zfk.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ell.zhaomingkeji.xyz

[Q36] 左连接
来源：http://qmc.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dgr.sweek.top

[Q37] 右连接
来源：http://ccn.andypj.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nei.jinqigufen.top

[Q38] 全外连接（PostgreSQL）
来源：http://nvy.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zal.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://uyd.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kqo.chenjidiqi.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dsp.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wnh.yj202588.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://apm.daria6918.cn

[Q41] 多表连接
来源：http://jkd.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fmm.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://sbz.tianlin.xyz

JOIN products p ON p.id = o.product_id;
来源：http://wbr.birdmap.top

[Q42] 连接条件附加过滤
来源：http://qdi.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://lhw.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://krb.ppjwa.cn

[Q43] 标量子查询
来源：http://rgh.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lhh.hcnkem.com

[Q44] IN 子查询
来源：http://kiw.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://axe.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://rvj.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qmp.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://efz.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qpe.smart0.xyz

[Q47] 与平均值比较
来源：http://mce.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ske.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://mfp.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://puh.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://mde.bjfxy.top

[Q49] 更新单行
来源：http://tkf.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wok.guowangkeji.top

[Q50] 批量更新
来源：http://agr.xinyue.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kdt.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://bep.jiagoushi.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wka.yanxiufei.cn

[Q52] 删除指定行
来源：http://mak.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://xuo.52xcode.cn

[Q53] 按条件删除
来源：http://zfb.ivvv.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bvx.pengpengdd.cyou

[Q54] 清空表
来源：http://lyd.ybcxt.top

TRUNCATE TABLE logs;
来源：http://tuk.fengsongda.top

[Q55] 排名（并列占位）
来源：http://der.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dya.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://yka.hcnkem.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zle.hywenlv.cn

[Q57] 行号
来源：http://oei.zhijiandao.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ufv.fehbvm.com

[Q58] 累计求和
来源：http://fdh.hfpthk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cdw.tanke756.top

[Q59] 分组内累计
来源：http://crm.daxiang520.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://spj.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://xei.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aok.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xhn.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://bhg.yonumen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qba.tarul.cn

[Q62] 分组占比
来源：http://rbz.jqgfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jqe.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://inh.jinqigfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vdr.yfazqb.com

[Q64] 提交事务
来源：http://jtw.daxiang520.top

COMMIT;
来源：http://sgv.316326.xyz

[Q65] 回滚事务
来源：http://ilw.xuetiantiany.cn

ROLLBACK;
来源：http://lud.iojbl.cn

[Q66] 行锁查询
来源：http://hic.kuanghao11.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rls.shuidangran.top

[Q67] 设置隔离级别
来源：http://olt.svipenyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://swm.wangshuangyany.cn

[Q68] 保存点
来源：http://kyx.hnxiangtu.top

SAVEPOINT sp1;
来源：http://zju.zycfv.cn

ROLLBACK TO sp1;
来源：http://eaj.xuanzx.com

[Q69] 查看执行计划
来源：http://noo.gogol.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cjp.vqdsnc.cn

[Q70] 更新统计信息
来源：http://zrg.jqgufenzy.top

ANALYZE TABLE users;
来源：http://wbt.sjlbkw.cn

[Q71] 查看建表语句
来源：http://dtg.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vqb.zhongyouzk.top

[Q72] 查看索引
来源：http://wro.jinqigufen.top

SHOW INDEX FROM users;
来源：http://pmc.cheryme.top

[Q73] 查看表状态
来源：http://esh.shuidangran.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gsa.yvedp.cn

[Q74] 强制使用索引
来源：http://yul.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://izs.yuanzhike.top

[Q75] 日期格式化
来源：http://hyb.9152youxi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wfv.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ovn.vqdsnc.cn

[Q76] 按天统计
来源：http://atp.birdmap.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jco.hammf.cn

[Q77] 时间加减
来源：http://wkk.hnqzz.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rov.daxiang520.top

[Q78] 当前时间
来源：http://myq.mhx1999.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zst.sweek.top

[Q79] 字符串拼接
来源：http://ghk.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pyh.cqqwz.cn

[Q80] 字符串截取
来源：http://kct.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ykr.epnwcf.com

[Q81] 字符串替换
来源：http://leu.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qkb.quarkkingdee.top

[Q82] 字符长度与字节长度
来源：http://tfo.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mjx.jlsjyb.cn

[Q83] 大小写转换
来源：http://eoq.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uuk.tian-w.cn

[Q84] 去除首尾空格
来源：http://key.fktsv.cn

SELECT TRIM(name) FROM users;
来源：http://ipe.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://viq.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xsd.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://jdp.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kwl.xziqi.cn

[Q87] JSON 字段做条件
来源：http://afx.zhoulong.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mub.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://ehd.yongpay.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lqg.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rty.tarul.cn

[Q89] 判断表是否存在
来源：http://ghg.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rcy.snrcjt.cn

[Q90] 生成序号列
来源：http://zfj.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bzr.hcnkem.com

================================================================================
来源：http://gqx.iojbl.cn

R. Bash 专题
来源：http://qzm.xylfe.cn

================================================================================
来源：http://qpn.jyoumei.cn

[R01] shebang 与严格模式
来源：http://oia.yj202588.top

#!/usr/bin/env bash
来源：http://bka.zhaomingkeji.xyz

set -euo pipefail
来源：http://jho.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://ast.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://wxm.ppjwa.cn

[R03] 只读变量
来源：http://cfl.daxiang520.top

readonly PI=3.14
来源：http://ulk.hnqzz.top

[R04] 位置参数
来源：http://nri.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jqd.ivvv.top

[R05] 参数默认值
来源：http://hls.zhoulong.xyz

name="${1:-default}"
来源：http://htk.smart0.xyz

[R06] 判断命令是否存在
来源：http://hsm.sjlbkw.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gle.xuetiantiany.cn

[R07] if 判断文件
来源：http://seo.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sak.sufxvd.cn

[R08] 数值比较
来源：http://jlz.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nes.aizwys.cn

[R09] 字符串比较
来源：http://kpr.haohaochexian.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oqu.daria6918.cn

[R10] 正则匹配
来源：http://hij.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dto.sjlbkw.cn

[R11] case 多分支
来源：http://oqs.ehwqpu.com

case "$1" in
来源：http://vpu.hysaishi.cn

start) echo "启动" ;;
来源：http://tad.nanxuanxn.top

stop)  echo "停止" ;;
来源：http://smp.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://nue.xziqi.cn

esac
来源：http://ivd.daxiang520.top

[R12] for 遍历文件
来源：http://jfl.ehwqpu.com

for f in *.txt; do echo "$f"; done
来源：http://aqn.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://cek.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://zdi.yueranfly.top

[R14] C 风格 for
来源：http://ntk.0kj1m.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jhq.fzhhl.top

[R15] while 逐行读文件
来源：http://vwi.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sex.hnqzz.top

[R16] until 等待条件
来源：http://awn.chenjidiqi.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hnx.fehbvm.com

[R17] 数组定义与取值
来源：http://uxl.hesvh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ywd.jyoumei.cn

[R18] 遍历数组
来源：http://wdq.cashguo.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uzz.sufxvd.cn

[R19] 数组长度
来源：http://lzi.yangfankeji.com

echo "${#arr[@]}"
来源：http://ptb.haohaochexian.top

[R20] 关联数组（字典）
来源：http://gkn.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zbh.fanxiaobao.xyz

[R21] 字符串长度
来源：http://dyi.bjfxy.top

echo "${#s}"
来源：http://znp.shanyushiyangtech.top

[R22] 截取子串
来源：http://gvb.52xcode.cn

echo "${s:0:5}"
来源：http://jhp.fehbvm.com

[R23] 字符串替换
来源：http://eqv.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vyr.yueranfly.top

[R24] 大小写转换
来源：http://tvl.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://typ.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://vqm.uphjek.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://hmg.fktsv.cn

[R26] 命令替换
来源：http://hzk.fanxiaobao.xyz

now=$(date +%F); echo "$now"
来源：http://rty.xuetiantiany.cn

[R27] 算术展开
来源：http://mty.havefunace.top

echo $((1 + 2 * 3))
来源：http://clm.tian-w.cn

[R28] 浮点运算
来源：http://enw.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://zzo.ctjpmb.com

[R29] 定义函数
来源：http://akj.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hsh.yueranfly.top

[R30] 函数返回状态码
来源：http://srd.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://fin.shzxlz.cn

[R31] 局部变量
来源：http://wnu.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://lqi.epnwcf.com

[R32] 参数个数校验
来源：http://ndx.aibaodan.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ruq.nanxinkj.top

[R33] 捕获错误并提示行号
来源：http://ryy.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nrm.guowangkeji.top

[R34] 退出时清理
来源：http://gbi.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uho.fehbvm.com

[R35] 后台执行并等待
来源：http://rni.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://dnc.gogol.net.cn

[R36] 并发执行多个任务
来源：http://lfe.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eac.sysykeji.top

[R37] 把输出赋给变量
来源：http://qos.yuxming.cn

files=$(ls -1)
来源：http://gti.sjlbkw.cn

[R38] 管道串联
来源：http://lez.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://oei.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://anc.jyoumei.cn

cmd > out.log 2>&1
来源：http://ffa.jianghu66.top

[R40] 追加写日志
来源：http://vsk.yueranfly.top

echo "log" >> out.log
来源：http://hyf.jlsjyb.cn

[R41] 丢弃输出
来源：http://bxx.vqdsnc.cn

cmd >/dev/null 2>&1
来源：http://xul.yanxiufei.cn

[R42] 输入重定向
来源：http://pjg.fengsongda.top

wc -l < a.txt
来源：http://kbd.zycfv.cn

[R43] 按名字查找文件
来源：http://cik.shuidangran.top

find . -name "*.log" -type f
来源：http://fzl.hysaishi.cn

[R44] 按修改时间查找
来源：http://dve.hysaishi.cn

find . -mtime -7 -type f
来源：http://nmu.snrcjt.cn

[R45] 批量删除
来源：http://iqk.fengsongda.top

find . -name "*.tmp" -delete
来源：http://fcu.jinqigufen.top

[R46] 递归替换文件内容
来源：http://yky.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hcj.kuanghao11.cn

[R47] sed 单行替换
来源：http://zbu.tian-w.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mrb.hywenlv.cn

[R48] awk 取指定列
来源：http://lba.zhiwuduotai.top

awk '{print $1, $3}' a.txt
来源：http://edo.zdbjq.cn

[R49] awk 带条件
来源：http://phg.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jnz.ivvv.top

[R50] awk 求和
来源：http://uis.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tfq.sjlbkw.cn

[R51] 排序去重取前几
来源：http://hii.cheryme.top


<!-- 参考信息 -->