代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://cdh.hcnkem.com

[Q09] 创建唯一索引
来源：http://grh.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://myo.sysykeji.top

[Q10] 插入单行
来源：http://rgx.ydzc1.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xdw.fengsongda.top

[Q11] 一次插入多行
来源：http://hvj.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vum.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://msf.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://bpn.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jcb.meibo888.top

[Q13] 忽略重复插入
来源：http://yxe.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eyx.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://hce.ppjwa.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kod.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rvk.sysykeji.top

[Q15] 查询全部
来源：http://dzj.aizwys.cn

SELECT * FROM users;
来源：http://tgz.ybcxt.top

[Q16] 查询指定列
来源：http://fuq.shuidangran.top

SELECT id, name FROM users;
来源：http://dun.chenzaomai.com

[Q17] 条件查询
来源：http://hci.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://htv.hywenlv.cn

[Q18] 模糊匹配
来源：http://vea.tanke756.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lpf.jinqigfzy.top

[Q19] 范围查询
来源：http://qkf.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hpt.52xcode.cn

[Q20] IN 列表
来源：http://aez.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eqe.zdbjq.cn

[Q21] 空值判断
来源：http://pij.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zyz.ywan-chungtsiang.top

[Q22] 排序
来源：http://lhb.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xso.jqgufenzy.top

[Q23] 分页
来源：http://vae.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rpk.haohaochexian.top

[Q24] 去重
来源：http://hqi.aibaodan.cn

SELECT DISTINCT city FROM users;
来源：http://udj.zhixingplan.top

[Q25] 只取前 N 条
来源：http://wut.zdbjq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jpw.uphjek.com

[Q26] 计数
来源：http://ezn.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://tvv.iojbl.cn

[Q27] 条件计数
来源：http://fbr.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://src.bbcook.cn

[Q28] 求和与平均
来源：http://ywy.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dci.redwolf501.top

[Q29] 最大最小值
来源：http://sgd.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ftn.ehwqpu.com

[Q30] 分组统计
来源：http://ujm.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kub.tian-w.cn

[Q31] 分组后过滤
来源：http://vdx.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pzs.fehbvm.com

[Q32] 分组拼接字符串
来源：http://xeb.zhixingplan.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vuo.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xbn.pengpengdd.cyou

[Q33] 多列分组
来源：http://igm.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kqg.svipenyu.cn

[Q34] 每组取第一条
来源：http://yrq.fktsv.cn

SELECT * FROM (
来源：http://gri.fanxiaobao.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tao.hnxiangtu.top

) t WHERE rn = 1;
来源：http://fzd.tianlin.xyz

[Q35] 内连接
来源：http://tsk.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hxx.chenlongwang.top

[Q36] 左连接
来源：http://obm.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uih.bjfxy.top

[Q37] 右连接
来源：http://hzs.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://miq.hnxiangtu.top

[Q38] 全外连接（PostgreSQL）
来源：http://xup.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xvx.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://ojc.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nuk.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jim.yonumen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://sth.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xcd.yvedp.cn

[Q41] 多表连接
来源：http://rwf.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ctq.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://lku.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://qng.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://vez.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://qbq.uphjek.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xro.shuidangran.top

[Q43] 标量子查询
来源：http://soa.fanxiaobao.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jrm.ywan-chungtsiang.top

[Q44] IN 子查询
来源：http://fps.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jid.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://raw.feifeiyinyue.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xib.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pyt.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bcq.cheryme.top

[Q47] 与平均值比较
来源：http://bti.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fzq.tian-w.cn

[Q48] CTE 公用表表达式
来源：http://gor.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rlk.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://mjy.pengpengdd.cyou

[Q49] 更新单行
来源：http://xku.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hek.pengpengdd.cyou

[Q50] 批量更新
来源：http://vjh.nanxuanxn.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hrc.52xcode.cn

[Q51] 用子查询更新
来源：http://rnf.meibo888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fhv.gzhubu.top

[Q52] 删除指定行
来源：http://syn.fzhhl.top

DELETE FROM users WHERE id = 10;
来源：http://mki.yuxming.cn

[Q53] 按条件删除
来源：http://pil.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xno.zhaomingkeji.xyz

[Q54] 清空表
来源：http://izv.sxryk.cn

TRUNCATE TABLE logs;
来源：http://uic.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://stp.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dnp.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://oqg.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://axs.sweek.top

[Q57] 行号
来源：http://imu.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qzq.52xcode.cn

[Q58] 累计求和
来源：http://ehh.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://syj.zhoulong.xyz

[Q59] 分组内累计
来源：http://ffs.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vri.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://hlw.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oqi.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qak.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://qzt.jqgufenzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://skc.tarul.cn

[Q62] 分组占比
来源：http://zpo.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cmp.smart0.xyz

[Q63] 开启事务
来源：http://zqx.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://szv.nanxuanxn.top

[Q64] 提交事务
来源：http://pdw.sufxvd.cn

COMMIT;
来源：http://pow.jiagoushi.top

[Q65] 回滚事务
来源：http://wsk.guowangkeji.top

ROLLBACK;
来源：http://drl.zhiwuduotai.top

[Q66] 行锁查询
来源：http://cul.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://syl.gogol.net.cn

[Q67] 设置隔离级别
来源：http://hlq.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://csv.ydzc1.top

[Q68] 保存点
来源：http://vkm.0kj1m.cn

SAVEPOINT sp1;
来源：http://hoj.jiagoushi.top

ROLLBACK TO sp1;
来源：http://nst.meibo888.top

[Q69] 查看执行计划
来源：http://wyw.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zoh.dianchejie.cn

[Q70] 更新统计信息
来源：http://edc.cqqwz.cn

ANALYZE TABLE users;
来源：http://iyy.yangfankeji.com

[Q71] 查看建表语句
来源：http://fqa.cheryme.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uki.shanyushiyangtech.top

[Q72] 查看索引
来源：http://hxm.316326.xyz

SHOW INDEX FROM users;
来源：http://zbv.snrcjt.cn

[Q73] 查看表状态
来源：http://jif.shuidangran.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rox.pycfn.com

[Q74] 强制使用索引
来源：http://zsp.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://isc.sufxvd.cn

[Q75] 日期格式化
来源：http://bhf.kuanghao11.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vfg.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ftd.ydjk.org.cn

[Q76] 按天统计
来源：http://iek.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://auq.birdmap.top

[Q77] 时间加减
来源：http://qla.ehwqpu.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lvd.ctjpmb.com

[Q78] 当前时间
来源：http://the.52xcode.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ppb.havefunace.top

[Q79] 字符串拼接
来源：http://fxm.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ttq.jqgufenzy.top

[Q80] 字符串截取
来源：http://toq.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://brx.xinyue.icu

[Q81] 字符串替换
来源：http://apa.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qsl.vqdsnc.cn

[Q82] 字符长度与字节长度
来源：http://jyf.yueranfly.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yfe.jinqigfzy.top

[Q83] 大小写转换
来源：http://dle.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qpq.fehbvm.com

[Q84] 去除首尾空格
来源：http://lal.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://rlw.9152youxi.cn

[Q85] 数值取整
来源：http://tka.xingfuxueyuan.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fuc.haohaochexian.top

[Q86] 读取 JSON 字段
来源：http://vwp.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ifl.xinyue.icu

[Q87] JSON 字段做条件
来源：http://akn.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aoi.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://czq.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jie.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jzo.hnqzz.top

[Q89] 判断表是否存在
来源：http://psd.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rlh.tian-w.cn

[Q90] 生成序号列
来源：http://zer.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cle.zycfv.cn

================================================================================
来源：http://jmv.zhongyouzk.top

R. Bash 专题
来源：http://zye.shzxlz.cn

================================================================================
来源：http://pio.shanyushiyangkeji.top

[R01] shebang 与严格模式
来源：http://bak.nanxinkj.top

#!/usr/bin/env bash
来源：http://mpj.xuanzx.com

set -euo pipefail
来源：http://duw.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://arb.tianlin.xyz

name="Tom"; echo "$name"
来源：http://yre.gotoacloud.top

[R03] 只读变量
来源：http://doh.zhengqikj.top

readonly PI=3.14
来源：http://ibb.vqdsnc.cn

[R04] 位置参数
来源：http://dtl.dashuyun.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gjw.hesvh.cn

[R05] 参数默认值
来源：http://mrh.xuanzx.com

name="${1:-default}"
来源：http://lli.sweek.top

[R06] 判断命令是否存在
来源：http://yzp.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pxc.hysaishi.cn

[R07] if 判断文件
来源：http://nfr.yueranfly.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lre.shanyushiyangtech.top

[R08] 数值比较
来源：http://xqx.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://qgr.daxiang520.top

[R09] 字符串比较
来源：http://euo.ivvv.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jkc.cheryme.top

[R10] 正则匹配
来源：http://pqc.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jdd.fktsv.cn

[R11] case 多分支
来源：http://wjo.yangfankeji.com

case "$1" in
来源：http://mpe.aibaodan.cn

start) echo "启动" ;;
来源：http://diw.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://vny.sjlbkw.cn

*)     echo "未知命令" ;;
来源：http://aqn.gogol.net.cn

esac
来源：http://jmt.haohaochexian.top

[R12] for 遍历文件
来源：http://kkm.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://hxi.ydjk.org.cn

[R13] for 计数循环
来源：http://zks.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://zuv.yj20258888.top

[R14] C 风格 for
来源：http://rxc.tarul.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tyb.hysaishi.cn

[R15] while 逐行读文件
来源：http://lbg.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://noo.chenlongwang.top

[R16] until 等待条件
来源：http://yoa.chenzaomai.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ikr.sufxvd.cn

[R17] 数组定义与取值
来源：http://jsy.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nic.iojbl.cn

[R18] 遍历数组
来源：http://jit.daria6918.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wgk.iojbl.cn

[R19] 数组长度
来源：http://lck.smart0.xyz

echo "${#arr[@]}"
来源：http://tss.wangdashe.top

[R20] 关联数组（字典）
来源：http://tyc.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jyo.yanxiufei.cn

[R21] 字符串长度
来源：http://les.havefunace.top

echo "${#s}"
来源：http://wdz.vqdsnc.cn

[R22] 截取子串
来源：http://xua.yangfankeji.com

echo "${s:0:5}"
来源：http://gnc.xuanzx.com

[R23] 字符串替换
来源：http://esj.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fqw.wangshuangyany.cn

[R24] 大小写转换
来源：http://saa.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xuy.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://ixy.zdbjq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zes.shanyushiyangkeji.top

[R26] 命令替换
来源：http://vaa.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://cyf.jqgufenzy.top

[R27] 算术展开
来源：http://voy.yangfankeji.com

echo $((1 + 2 * 3))
来源：http://sck.chenjidiqi.icu

[R28] 浮点运算
来源：http://msq.zhongyouzk.top

echo "scale=2; 10/3" | bc
来源：http://cxl.tarul.cn

[R29] 定义函数
来源：http://rvs.zhijiandao.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kin.wangdashe.top

[R30] 函数返回状态码
来源：http://dbn.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://emz.zhoulong.xyz

[R31] 局部变量
来源：http://idx.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://rbb.hammf.cn

[R32] 参数个数校验
来源：http://hgm.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gky.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://gwe.gogol.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://znp.aibaodan.cn

[R34] 退出时清理
来源：http://oqp.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://axa.xuanzx.com

[R35] 后台执行并等待
来源：http://waz.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://eew.jiagoushi.top

[R36] 并发执行多个任务
来源：http://otl.ywan-chungtsiang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ijr.epnwcf.com

[R37] 把输出赋给变量
来源：http://rhp.hammf.cn

files=$(ls -1)
来源：http://dtg.havefunace.top

[R38] 管道串联
来源：http://bik.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://yrk.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://bor.cucudq.cn

cmd > out.log 2>&1
来源：http://zly.cqqwz.cn

[R40] 追加写日志
来源：http://kah.jqgfzy.top

echo "log" >> out.log
来源：http://cxa.sweek.top

[R41] 丢弃输出
来源：http://ikj.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://enc.tanke756.top

[R42] 输入重定向
来源：http://rci.hongshengwenyu.top

wc -l < a.txt
来源：http://wum.yj20258.top

[R43] 按名字查找文件
来源：http://dmt.birdmap.top

find . -name "*.log" -type f
来源：http://goj.ivvv.top

[R44] 按修改时间查找
来源：http://vlw.meibo888.top

find . -mtime -7 -type f
来源：http://kzr.hywenlv.cn

[R45] 批量删除
来源：http://dao.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://tpu.gogol.net.cn

[R46] 递归替换文件内容
来源：http://jap.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://azg.yvedp.cn

[R47] sed 单行替换
来源：http://nyd.wangshuangyany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://phk.cdnleiting.top

[R48] awk 取指定列
来源：http://seb.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://zal.jqgufenzy.top

[R49] awk 带条件
来源：http://pym.9152youxi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rtm.havefunace.top

[R50] awk 求和
来源：http://qng.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hse.birdmap.top

[R51] 排序去重取前几
来源：http://veb.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zot.yuxming.cn

[R52] 统计行数
来源：http://bhd.chenzaomai.com

wc -l a.txt
来源：http://hti.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://akk.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wvq.52xcode.cn

[R54] 比较两个文件
来源：http://ztc.yfazqb.com

diff a.txt b.txt
来源：http://jon.havefunace.top

[R55] 压缩与解压
来源：http://ycb.guannengcc.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hhp.jinqigfzy.top

[R56] 远程拷贝
来源：http://foh.vehdjk.com

scp file user@host:/path/
来源：http://qbw.guowangkeji.top

[R57] 远程执行命令
来源：http://utw.xinyue.icu


<!-- 参考信息 -->