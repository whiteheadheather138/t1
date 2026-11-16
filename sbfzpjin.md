代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yzy.9152youxi.cn

[Q11] 一次插入多行
来源：http://ezg.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gwq.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://wuu.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pys.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hlw.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://mnq.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://poh.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://eyh.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cgz.tianlin.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gdc.andypj.xyz

[Q15] 查询全部
来源：http://dhd.sufxvd.cn

SELECT * FROM users;
来源：http://gxk.c1oappe.top

[Q16] 查询指定列
来源：http://xny.ybcxt.top

SELECT id, name FROM users;
来源：http://dme.ppjwa.cn

[Q17] 条件查询
来源：http://dot.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wtv.redwolf501.top

[Q18] 模糊匹配
来源：http://yfz.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pew.sjlbkw.cn

[Q19] 范围查询
来源：http://swp.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://slc.quarkkingdee.top

[Q20] IN 列表
来源：http://ldl.uphjek.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nxy.zycfv.cn

[Q21] 空值判断
来源：http://ssc.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hhd.svipenyu.cn

[Q22] 排序
来源：http://hcc.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lgt.gaohongyu789.top

[Q23] 分页
来源：http://bbq.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://auj.quarkkingdee.top

[Q24] 去重
来源：http://byc.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://jzw.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://gek.xylfe.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pza.ydjk.org.cn

[Q26] 计数
来源：http://ade.zycfv.cn

SELECT COUNT(*) FROM users;
来源：http://jmf.snrcjt.cn

[Q27] 条件计数
来源：http://gcd.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://duj.svipenyu.cn

[Q28] 求和与平均
来源：http://oqe.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fpy.shangyingyoupin.top

[Q29] 最大最小值
来源：http://sfr.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gqg.yanxiufei.cn

[Q30] 分组统计
来源：http://gfq.yuxming.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kzn.yj20258888.top

[Q31] 分组后过滤
来源：http://dqg.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kwx.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://sjy.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rhe.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dyx.xingfuxueyuan.xyz

[Q33] 多列分组
来源：http://gfc.ybcxt.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tmk.jinqigfzy.top

[Q34] 每组取第一条
来源：http://rqs.daxiang520.top

SELECT * FROM (
来源：http://twy.fanxiaobao.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pyi.iojbl.cn

) t WHERE rn = 1;
来源：http://gca.yuanzhike.top

[Q35] 内连接
来源：http://ern.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jmn.tarul.cn

[Q36] 左连接
来源：http://osl.vehdjk.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aig.hnxiangtu.top

[Q37] 右连接
来源：http://rtf.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ydp.316326.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://thl.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yaj.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://mkq.gzhubu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://exx.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nxy.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ugm.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://igu.cucudq.cn

[Q41] 多表连接
来源：http://tzt.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://txa.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://ugg.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://rfd.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://hny.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://bfd.hfpthk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lhn.sweek.top

[Q43] 标量子查询
来源：http://glp.pycfn.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xba.nanxinkj.top

[Q44] IN 子查询
来源：http://agn.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zna.pycfn.com

[Q45] EXISTS 判断存在
来源：http://nah.xylfe.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fyo.ydzc1.top

[Q46] NOT EXISTS 判断不存在
来源：http://xje.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://otl.yj20258888.top

[Q47] 与平均值比较
来源：http://oox.nwbrower.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ziw.gotoacloud.top

[Q48] CTE 公用表表达式
来源：http://bzc.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hqt.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://evt.hfpthk.cn

[Q49] 更新单行
来源：http://cdm.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hhs.chenlongwang.top

[Q50] 批量更新
来源：http://qyv.hnqzz.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://icz.wangdashe.top

[Q51] 用子查询更新
来源：http://dxc.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://npn.sufxvd.cn

[Q52] 删除指定行
来源：http://kez.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://dwt.feifeiyinyue.top

[Q53] 按条件删除
来源：http://oik.xingfuxueyuan.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qsj.xuanzx.com

[Q54] 清空表
来源：http://ouw.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://dmv.hammf.cn

[Q55] 排名（并列占位）
来源：http://cpu.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://udp.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://zzg.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://otu.316326.xyz

[Q57] 行号
来源：http://fcp.dianchejie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eky.pycfn.com

[Q58] 累计求和
来源：http://dhx.yanxiufei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://awk.shzxlz.cn

[Q59] 分组内累计
来源：http://lmi.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ico.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://bjr.hfpthk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wfq.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pue.ydzc1.top

[Q61] 移动平均
来源：http://wja.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zor.ppjwa.cn

[Q62] 分组占比
来源：http://dck.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://etk.feifeiyinyue.top

[Q63] 开启事务
来源：http://tdv.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vhm.xuanzx.com

[Q64] 提交事务
来源：http://air.zdbjq.cn

COMMIT;
来源：http://yzd.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://myo.zhoulong.xyz

ROLLBACK;
来源：http://psk.xylfe.cn

[Q66] 行锁查询
来源：http://frt.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bih.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://woa.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ens.yuanzhike.top

[Q68] 保存点
来源：http://ljk.yangfankeji.com

SAVEPOINT sp1;
来源：http://ddv.hnqzz.top

ROLLBACK TO sp1;
来源：http://cpi.mhx1999.top

[Q69] 查看执行计划
来源：http://wbg.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fsv.redwolf501.top

[Q70] 更新统计信息
来源：http://gzk.shuidangran.top

ANALYZE TABLE users;
来源：http://evx.c1oappe.top

[Q71] 查看建表语句
来源：http://qym.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rxm.sxryk.cn

[Q72] 查看索引
来源：http://zlk.iojbl.cn

SHOW INDEX FROM users;
来源：http://ear.yonumen.top

[Q73] 查看表状态
来源：http://olf.hesvh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zlx.birdmap.top

[Q74] 强制使用索引
来源：http://uon.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qvt.ydzc1.top

[Q75] 日期格式化
来源：http://pta.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vxz.yangfankeji.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://roh.gogol.net.cn

[Q76] 按天统计
来源：http://xtf.tanke756.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://czl.dianchejie.cn

[Q77] 时间加减
来源：http://aix.316326.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dgp.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://arj.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://spd.vqdsnc.cn

[Q79] 字符串拼接
来源：http://obz.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kas.uphjek.com

[Q80] 字符串截取
来源：http://trs.yonumen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dnn.hysaishi.cn

[Q81] 字符串替换
来源：http://zkj.hywenlv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gwj.sjlbkw.cn

[Q82] 字符长度与字节长度
来源：http://drh.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hne.mhx1999.top

[Q83] 大小写转换
来源：http://wjc.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bkz.yj202588.top

[Q84] 去除首尾空格
来源：http://jiz.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://zyq.zhengqikj.top

[Q85] 数值取整
来源：http://qpr.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hyq.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://pvn.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tlf.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://jln.bjfxy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://efp.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://plh.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://guo.zdqjudy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xwk.52xcode.cn

[Q89] 判断表是否存在
来源：http://aoq.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cxz.zhaomingkeji.xyz

[Q90] 生成序号列
来源：http://uxr.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jfb.fanxiaobao.xyz

================================================================================
来源：http://tuy.jqgufenzy.top

R. Bash 专题
来源：http://vmx.ppjwa.cn

================================================================================
来源：http://tqt.nwbrower.top

[R01] shebang 与严格模式
来源：http://lxq.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://ulp.fzhhl.top

set -euo pipefail
来源：http://pqf.xylfe.cn

[R02] 变量赋值与使用
来源：http://vey.dianchejie.cn

name="Tom"; echo "$name"
来源：http://kvz.c1oappe.top

[R03] 只读变量
来源：http://mkd.daxiang520.top

readonly PI=3.14
来源：http://nld.jlsjyb.cn

[R04] 位置参数
来源：http://lam.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://end.jqgufenzy.top

[R05] 参数默认值
来源：http://yzh.jinghuilouyu.cn

name="${1:-default}"
来源：http://nzc.xylfe.cn

[R06] 判断命令是否存在
来源：http://wyp.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yad.wangdashe.top

[R07] if 判断文件
来源：http://gnt.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tmj.tanke756.top

[R08] 数值比较
来源：http://efi.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mcv.shzxlz.cn

[R09] 字符串比较
来源：http://xeb.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://soe.dashuyun.cn

[R10] 正则匹配
来源：http://edj.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yyf.tarul.cn

[R11] case 多分支
来源：http://nvw.wangshuangyany.cn

case "$1" in
来源：http://jrj.yj202588.top

start) echo "启动" ;;
来源：http://cee.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://kws.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://lkj.smart0.xyz

esac
来源：http://hgx.shangyingyoupin.top

[R12] for 遍历文件
来源：http://nye.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://yct.fktsv.cn

[R13] for 计数循环
来源：http://qqz.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://cby.ppjwa.cn

[R14] C 风格 for
来源：http://msq.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://awl.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://fgr.vehdjk.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hjv.nanxinkj.top

[R16] until 等待条件
来源：http://mdx.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jxv.ydjk.org.cn

[R17] 数组定义与取值
来源：http://awl.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ffb.xingfuxueyuan.xyz

[R18] 遍历数组
来源：http://lva.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sqn.pycfn.com

[R19] 数组长度
来源：http://ixa.wangdashe.top

echo "${#arr[@]}"
来源：http://nyw.havefunace.top

[R20] 关联数组（字典）
来源：http://eam.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bcy.guannengcc.top

[R21] 字符串长度
来源：http://pof.zhoulong.xyz

echo "${#s}"
来源：http://tyy.cashguo.top

[R22] 截取子串
来源：http://kid.0kj1m.cn

echo "${s:0:5}"
来源：http://iiv.fehbvm.com

[R23] 字符串替换
来源：http://wbb.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hgd.cdnleiting.top

[R24] 大小写转换
来源：http://jbk.ctjpmb.com

echo "${s^^}"; echo "${s,,}"
来源：http://xes.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://lah.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gfu.fanxiaobao.xyz

[R26] 命令替换
来源：http://yqy.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://qgq.hfpthk.cn

[R27] 算术展开
来源：http://rzg.xuanzx.com

echo $((1 + 2 * 3))
来源：http://zap.jianghu66.top

[R28] 浮点运算
来源：http://dkv.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://xwb.zhixingplan.top

[R29] 定义函数
来源：http://uvn.zhijiandao.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ayg.wangdashe.top

[R30] 函数返回状态码
来源：http://azq.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://ngl.yueranfly.top

[R31] 局部变量
来源：http://hhf.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://kbc.zdbjq.cn

[R32] 参数个数校验
来源：http://pgk.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://syh.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://saz.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://obg.vqdsnc.cn

[R34] 退出时清理
来源：http://amo.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cek.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://gsr.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://cfd.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://txk.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://svz.gogol.net.cn

[R37] 把输出赋给变量
来源：http://tnq.ctjpmb.com

files=$(ls -1)
来源：http://otl.yangfankeji.com

[R38] 管道串联
来源：http://gju.fzhhl.top

cat a.txt | grep -i error | wc -l
来源：http://lec.yj20258.top

[R39] 重定向标准输出与错误
来源：http://fly.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://zbn.daria6918.cn

[R40] 追加写日志
来源：http://qdo.havefunace.top

echo "log" >> out.log
来源：http://xsq.jlsjyb.cn

[R41] 丢弃输出
来源：http://xfe.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://fig.sufxvd.cn

[R42] 输入重定向
来源：http://iqk.jyoumei.cn

wc -l < a.txt
来源：http://ued.gzhubu.top

[R43] 按名字查找文件
来源：http://aeb.mhx1999.top

find . -name "*.log" -type f
来源：http://srx.bjfxy.top

[R44] 按修改时间查找
来源：http://axv.nwbrower.top

find . -mtime -7 -type f
来源：http://ltj.xuetiantiany.cn

[R45] 批量删除
来源：http://pkn.ydzc1.top

find . -name "*.tmp" -delete
来源：http://omx.cashguo.top

[R46] 递归替换文件内容
来源：http://ape.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jsh.jinqigfzy.top

[R47] sed 单行替换
来源：http://pce.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kex.hysaishi.cn

[R48] awk 取指定列
来源：http://knx.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://axx.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://zfm.uphjek.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yvr.nwbrower.top

[R50] awk 求和
来源：http://ism.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://eqt.zycfv.cn

[R51] 排序去重取前几
来源：http://pvi.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pmc.chenjidiqi.icu

[R52] 统计行数
来源：http://zhi.dianchejie.cn

wc -l a.txt
来源：http://oyr.aizwys.cn

[R53] 查看文件头与实时尾
来源：http://jwl.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qhr.fktsv.cn

[R54] 比较两个文件
来源：http://vjc.cashguo.top

diff a.txt b.txt
来源：http://qyr.ivvv.top

[R55] 压缩与解压
来源：http://ufn.yangfankeji.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mlk.svipenyu.cn

[R56] 远程拷贝
来源：http://edr.guowangkeji.top

scp file user@host:/path/
来源：http://rmp.shzxlz.cn

[R57] 远程执行命令
来源：http://bom.nwbrower.top

ssh user@host 'uptime'
来源：http://nxe.tanke756.top

[R58] 下载文件
来源：http://hnp.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qcz.hysaishi.cn

[R59] 发 POST JSON
来源：http://txd.zhoulong.xyz


<!-- 参考信息 -->