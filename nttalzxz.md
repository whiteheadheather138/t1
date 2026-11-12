代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rbg.birdmap.top

user_id INT NOT NULL,
来源：http://fnh.yvedp.cn

amount DECIMAL(10, 2),
来源：http://xfv.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xcu.uphjek.com

);
来源：http://nrd.jqgfzy.top

[Q03] 增加列
来源：http://znf.iojbl.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rbc.svipenyu.cn

[Q04] 修改列类型
来源：http://wgr.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pzr.sjlbkw.cn

[Q05] 重命名列
来源：http://iwb.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zgy.mhx1999.top

[Q06] 删除列
来源：http://ryc.redwolf501.top

ALTER TABLE users DROP COLUMN age;
来源：http://lak.zdbjq.cn

[Q07] 删除表
来源：http://fof.9152youxi.cn

DROP TABLE IF EXISTS orders;
来源：http://uin.zhiwuduotai.top

[Q08] 创建普通索引
来源：http://dbx.shanyushiyangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hbg.birdmap.top

[Q09] 创建唯一索引
来源：http://sbo.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://asx.snrcjt.cn

[Q10] 插入单行
来源：http://pul.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jqk.chenlongwang.top

[Q11] 一次插入多行
来源：http://nei.meibo888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ovj.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://kac.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://vdc.bjfxy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uyo.ydzc1.top

[Q13] 忽略重复插入
来源：http://zvj.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://npa.hywenlv.cn

[Q14] 存在则更新（upsert）
来源：http://fzm.hnxiangtu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ykc.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rmx.jinqigfzy.top

[Q15] 查询全部
来源：http://don.cashguo.top

SELECT * FROM users;
来源：http://tmo.vqdsnc.cn

[Q16] 查询指定列
来源：http://cbd.zhijiandao.cn

SELECT id, name FROM users;
来源：http://jxe.zdqjudy.top

[Q17] 条件查询
来源：http://qgt.uphjek.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kpl.sufxvd.cn

[Q18] 模糊匹配
来源：http://ymq.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mdr.zhijiandao.cn

[Q19] 范围查询
来源：http://ufs.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wbp.ppjwa.cn

[Q20] IN 列表
来源：http://zme.ydjk.org.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ore.yj202588.top

[Q21] 空值判断
来源：http://prb.quarkkingdee.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rxh.yuanzhike.top

[Q22] 排序
来源：http://icc.ivvv.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mso.shanyushiyangtech.top

[Q23] 分页
来源：http://tdi.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vbs.mhx1999.top

[Q24] 去重
来源：http://hhb.xziqi.cn

SELECT DISTINCT city FROM users;
来源：http://vxs.daxiang520.top

[Q25] 只取前 N 条
来源：http://eig.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ath.yj20258888.top

[Q26] 计数
来源：http://sjt.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://rju.xylfe.cn

[Q27] 条件计数
来源：http://qnh.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bbd.chenzaomai.com

[Q28] 求和与平均
来源：http://fal.cucudq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eiw.hfpthk.cn

[Q29] 最大最小值
来源：http://jjv.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zrj.hesvh.cn

[Q30] 分组统计
来源：http://jml.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hfg.ppjwa.cn

[Q31] 分组后过滤
来源：http://qsa.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mfa.xziqi.cn

[Q32] 分组拼接字符串
来源：http://qft.aibaodan.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ryq.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://crj.chenzaomai.com

[Q33] 多列分组
来源：http://mul.yfazqb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mob.redwolf501.top

[Q34] 每组取第一条
来源：http://ojh.meibo888.top

SELECT * FROM (
来源：http://fcv.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ova.yueranfly.top

) t WHERE rn = 1;
来源：http://nhs.yanxiufei.cn

[Q35] 内连接
来源：http://lrx.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hdv.zycfv.cn

[Q36] 左连接
来源：http://ypm.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nkn.cheryme.top

[Q37] 右连接
来源：http://wmp.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ytq.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jjs.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uni.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://zdx.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ndq.epnwcf.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jel.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nan.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wga.mhx1999.top

[Q41] 多表连接
来源：http://sdo.shuidangran.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yaf.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://wuw.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://uod.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://ctv.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://pwg.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nsq.smart0.xyz

[Q43] 标量子查询
来源：http://zso.zdqjudy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rfw.9152youxi.cn

[Q44] IN 子查询
来源：http://jrs.vehdjk.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ecg.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://gts.jinqigufen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mfp.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tlu.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iso.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://wxv.cashguo.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gkk.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://fto.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cwq.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://ywc.c1oappe.top

[Q49] 更新单行
来源：http://ihv.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fuy.hnqzz.top

[Q50] 批量更新
来源：http://wjw.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rtu.aibaodan.cn

[Q51] 用子查询更新
来源：http://xro.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wqd.sjlbkw.cn

[Q52] 删除指定行
来源：http://juf.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://ylr.yangfankeji.com

[Q53] 按条件删除
来源：http://eae.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yjo.fehbvm.com

[Q54] 清空表
来源：http://hkf.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://rbw.bbcook.cn

[Q55] 排名（并列占位）
来源：http://gyr.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jcu.jiagoushi.top

[Q56] 密集排名（并列不占位）
来源：http://ezb.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://slh.yonumen.top

[Q57] 行号
来源：http://tdr.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ldk.wangshuangyany.cn

[Q58] 累计求和
来源：http://wot.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mmj.yangfankeji.com

[Q59] 分组内累计
来源：http://fwp.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vth.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://zgc.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xip.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://krf.316326.xyz

[Q61] 移动平均
来源：http://edh.yueranfly.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rms.dashuyun.cn

[Q62] 分组占比
来源：http://lrv.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pxm.sufxvd.cn

[Q63] 开启事务
来源：http://agt.zdbjq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ama.smart0.xyz

[Q64] 提交事务
来源：http://ddm.fengsongda.top

COMMIT;
来源：http://vav.aizwys.cn

[Q65] 回滚事务
来源：http://npv.xuanzx.com

ROLLBACK;
来源：http://lwh.svipenyu.cn

[Q66] 行锁查询
来源：http://els.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://biq.ybcxt.top

[Q67] 设置隔离级别
来源：http://wwb.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eow.haohaochexian.top

[Q68] 保存点
来源：http://atp.jinghuilouyu.cn

SAVEPOINT sp1;
来源：http://xuc.shanyushiyangtech.top

ROLLBACK TO sp1;
来源：http://krr.fzhhl.top

[Q69] 查看执行计划
来源：http://fma.yj20258.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iqr.sxryk.cn

[Q70] 更新统计信息
来源：http://vzp.uphjek.com

ANALYZE TABLE users;
来源：http://qzk.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://qsf.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cpf.ydzc1.top

[Q72] 查看索引
来源：http://fmr.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://pzz.havefunace.top

[Q73] 查看表状态
来源：http://xhk.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dla.hammf.cn

[Q74] 强制使用索引
来源：http://hsu.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oyd.shangyingyoupin.top

[Q75] 日期格式化
来源：http://hqk.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cpd.jyoumei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://trr.gotoacloud.top

[Q76] 按天统计
来源：http://qqx.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://myq.yj20258.top

[Q77] 时间加减
来源：http://jbz.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://voy.aibaodan.cn

[Q78] 当前时间
来源：http://ueg.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rum.zhijiandao.cn

[Q79] 字符串拼接
来源：http://asv.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jzd.nanxuanxn.top

[Q80] 字符串截取
来源：http://otj.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uti.gogol.net.cn

[Q81] 字符串替换
来源：http://low.guowangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eis.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://jsf.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vkd.tian-w.cn

[Q83] 大小写转换
来源：http://kfn.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gag.vqdsnc.cn

[Q84] 去除首尾空格
来源：http://xbd.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://fcp.ppjwa.cn

[Q85] 数值取整
来源：http://bhr.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zzs.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://ihz.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kxg.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://wkx.bjfxy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rqj.sysykeji.top

[Q88] 行转列（条件聚合）
来源：http://xpr.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tjk.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cfh.nanxinkj.top

[Q89] 判断表是否存在
来源：http://qpj.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uws.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://jkj.hnxiangtu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hlx.sufxvd.cn

================================================================================
来源：http://iui.gzhubu.top

R. Bash 专题
来源：http://myj.pengpengdd.cyou

================================================================================
来源：http://ulp.fanxiaobao.xyz

[R01] shebang 与严格模式
来源：http://srt.ybcxt.top

#!/usr/bin/env bash
来源：http://iqc.cdnleiting.top

set -euo pipefail
来源：http://ekn.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://ytd.zycfv.cn

name="Tom"; echo "$name"
来源：http://ydf.hnxiangtu.top

[R03] 只读变量
来源：http://tzd.hammf.cn

readonly PI=3.14
来源：http://kdr.xuetiantiany.cn

[R04] 位置参数
来源：http://krx.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eta.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://vqw.quarkkingdee.top

name="${1:-default}"
来源：http://sax.yj20258888.top

[R06] 判断命令是否存在
来源：http://oaz.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://czp.quarkkingdee.top

[R07] if 判断文件
来源：http://erp.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qug.guowangkeji.top

[R08] 数值比较
来源：http://jsm.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://tow.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://lxj.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xpz.yj202588.top

[R10] 正则匹配
来源：http://rkz.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rkk.smart0.xyz

[R11] case 多分支
来源：http://elp.hammf.cn

case "$1" in
来源：http://svd.havefunace.top

start) echo "启动" ;;
来源：http://bin.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://xio.bjfxy.top

*)     echo "未知命令" ;;
来源：http://llx.yj20258.top

esac
来源：http://nww.bjfxy.top

[R12] for 遍历文件
来源：http://yyh.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://kgm.shanyushiyangtech.top

[R13] for 计数循环
来源：http://cck.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://sqm.zhongyouzk.top

[R14] C 风格 for
来源：http://vkw.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hfy.yangfankeji.com

[R15] while 逐行读文件
来源：http://ddg.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hlf.jyoumei.cn

[R16] until 等待条件
来源：http://pni.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hgq.xuanzx.com

[R17] 数组定义与取值
来源：http://ahj.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://ilj.zhoulong.xyz

[R18] 遍历数组
来源：http://kwi.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jzh.xziqi.cn

[R19] 数组长度
来源：http://rvn.xuanzx.com

echo "${#arr[@]}"
来源：http://mfu.mhx1999.top

[R20] 关联数组（字典）
来源：http://kty.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zvl.hammf.cn

[R21] 字符串长度
来源：http://wmx.gotoacloud.top

echo "${#s}"
来源：http://ocx.ydzc1.top

[R22] 截取子串
来源：http://bby.ivvv.top

echo "${s:0:5}"
来源：http://sqt.ydjk.org.cn

[R23] 字符串替换
来源：http://yku.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jza.shuidangran.top

[R24] 大小写转换
来源：http://fqw.jqgufenzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://xwg.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://hkk.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wdo.guowangkeji.top

[R26] 命令替换
来源：http://dfi.xinyue.icu

now=$(date +%F); echo "$now"
来源：http://lsv.jqgufenzy.top

[R27] 算术展开
来源：http://eea.bjfxy.top

echo $((1 + 2 * 3))
来源：http://gub.tarul.cn

[R28] 浮点运算
来源：http://mlk.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://vfe.jianghu66.top

[R29] 定义函数
来源：http://lqq.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ydm.iojbl.cn

[R30] 函数返回状态码
来源：http://hky.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://hcn.cashguo.top

[R31] 局部变量
来源：http://kyu.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://zzx.snrcjt.cn

[R32] 参数个数校验
来源：http://ead.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qpc.ivvv.top

[R33] 捕获错误并提示行号
来源：http://jpz.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://niq.quarkkingdee.top

[R34] 退出时清理
来源：http://fsn.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://asq.cheryme.top

[R35] 后台执行并等待
来源：http://qxf.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ssh.jiagoushi.top

[R36] 并发执行多个任务
来源：http://swf.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fyy.yonumen.top

[R37] 把输出赋给变量
来源：http://xei.vqdsnc.cn

files=$(ls -1)
来源：http://fob.jinqigfzy.top

[R38] 管道串联
来源：http://gwk.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://vxl.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://qpi.tarul.cn

cmd > out.log 2>&1
来源：http://tnp.nwbrower.top

[R40] 追加写日志
来源：http://rxy.zhongyouzk.top

echo "log" >> out.log
来源：http://edm.jiagoushi.top

[R41] 丢弃输出
来源：http://xdu.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://ubc.zhoulong.xyz

[R42] 输入重定向
来源：http://edt.hysaishi.cn

wc -l < a.txt
来源：http://wjh.gzhubu.top

[R43] 按名字查找文件
来源：http://fiz.smart0.xyz

find . -name "*.log" -type f
来源：http://obw.tianlin.xyz

[R44] 按修改时间查找
来源：http://khy.zdbjq.cn

find . -mtime -7 -type f
来源：http://xxh.316326.xyz

[R45] 批量删除
来源：http://tzk.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://sze.hnqzz.top

[R46] 递归替换文件内容
来源：http://uyz.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ksz.feifeiyinyue.top

[R47] sed 单行替换
来源：http://gbt.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yrx.jyoumei.cn

[R48] awk 取指定列
来源：http://ggd.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://goc.ivvv.top

[R49] awk 带条件
来源：http://pwl.ppjwa.cn


<!-- 参考信息 -->