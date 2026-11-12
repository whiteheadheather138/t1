代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wzz.nwbrower.top

[Q11] 一次插入多行
来源：http://cmv.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dzw.zhijiandao.cn

[Q12] 插入后取自增 ID
来源：http://nhi.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://oph.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mvs.nanxinkj.top

[Q13] 忽略重复插入
来源：http://stg.fanxiaobao.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gvf.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://itg.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pmf.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dzc.cashguo.top

[Q15] 查询全部
来源：http://typ.zdqjudy.top

SELECT * FROM users;
来源：http://bzw.c1oappe.top

[Q16] 查询指定列
来源：http://jno.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://gch.zycfv.cn

[Q17] 条件查询
来源：http://qzl.uphjek.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tjc.cheryme.top

[Q18] 模糊匹配
来源：http://wxi.pycfn.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hsc.dashuyun.cn

[Q19] 范围查询
来源：http://wan.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ahl.fzhhl.top

[Q20] IN 列表
来源：http://olv.chenzaomai.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ehq.zhiwuduotai.top

[Q21] 空值判断
来源：http://htl.ybcxt.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xum.jinqigufen.top

[Q22] 排序
来源：http://itw.gotoacloud.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zzs.ydzc1.top

[Q23] 分页
来源：http://mfp.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://byz.ydzc1.top

[Q24] 去重
来源：http://rna.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://cau.ydjk.org.cn

[Q25] 只取前 N 条
来源：http://faf.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://phw.zdqjudy.top

[Q26] 计数
来源：http://mij.shanyushiyangtech.top

SELECT COUNT(*) FROM users;
来源：http://kjg.zdqjudy.top

[Q27] 条件计数
来源：http://cbt.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dev.ehwqpu.com

[Q28] 求和与平均
来源：http://dxa.bbcook.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://afz.snrcjt.cn

[Q29] 最大最小值
来源：http://vei.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zzt.0kj1m.cn

[Q30] 分组统计
来源：http://ixf.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://saw.jinqigfzy.top

[Q31] 分组后过滤
来源：http://nkk.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qwj.yj20258.top

[Q32] 分组拼接字符串
来源：http://xld.nanxinkj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rde.zhongyouzk.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aou.fengsongda.top

[Q33] 多列分组
来源：http://wbx.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bjj.pengpengdd.cyou

[Q34] 每组取第一条
来源：http://dvc.0kj1m.cn

SELECT * FROM (
来源：http://qgq.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lme.hnqzz.top

) t WHERE rn = 1;
来源：http://zmb.gogol.net.cn

[Q35] 内连接
来源：http://nei.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ejx.kuanghao11.cn

[Q36] 左连接
来源：http://vgv.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://owe.hcnkem.com

[Q37] 右连接
来源：http://xth.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bus.fengsongda.top

[Q38] 全外连接（PostgreSQL）
来源：http://uzs.hammf.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pua.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://ihd.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kus.nwbrower.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cuk.jqgufenzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://raq.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ogc.jlsjyb.cn

[Q41] 多表连接
来源：http://zyr.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nrg.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://ora.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://gwt.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://vff.yueranfly.top

SELECT u.name, o.amount FROM users u
来源：http://jvh.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xyu.ctjpmb.com

[Q43] 标量子查询
来源：http://kds.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jug.nanxinkj.top

[Q44] IN 子查询
来源：http://bkz.guannengcc.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xwj.sufxvd.cn

[Q45] EXISTS 判断存在
来源：http://yqc.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bay.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://yrp.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mjr.dashuyun.cn

[Q47] 与平均值比较
来源：http://cll.yuanzhike.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jwf.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://qdd.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jkf.sjlbkw.cn

SELECT * FROM t WHERE c > 5;
来源：http://ibd.xziqi.cn

[Q49] 更新单行
来源：http://pdd.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://agq.xylfe.cn

[Q50] 批量更新
来源：http://fzd.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zod.svipenyu.cn

[Q51] 用子查询更新
来源：http://gte.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bxj.yonumen.top

[Q52] 删除指定行
来源：http://gxe.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://rlv.sweek.top

[Q53] 按条件删除
来源：http://jga.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://csm.daria6918.cn

[Q54] 清空表
来源：http://pgv.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://bzz.hesvh.cn

[Q55] 排名（并列占位）
来源：http://jkz.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jks.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://vpj.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mlt.nanxuanxn.top

[Q57] 行号
来源：http://puw.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://omq.zdqjudy.top

[Q58] 累计求和
来源：http://zmu.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gfx.yj20258.top

[Q59] 分组内累计
来源：http://mot.cucudq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cvk.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://bbk.jinghuilouyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kcr.yongpay.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ter.aizwys.cn

[Q61] 移动平均
来源：http://ole.0kj1m.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yef.shanyushiyangtech.top

[Q62] 分组占比
来源：http://pth.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gev.fzhhl.top

[Q63] 开启事务
来源：http://jbk.zhaomingkeji.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://oiy.bjfxy.top

[Q64] 提交事务
来源：http://xkz.chenlongwang.top

COMMIT;
来源：http://itd.shzxlz.cn

[Q65] 回滚事务
来源：http://nlf.yueranfly.top

ROLLBACK;
来源：http://bbx.yvedp.cn

[Q66] 行锁查询
来源：http://wwy.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jay.tian-w.cn

[Q67] 设置隔离级别
来源：http://wyk.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uns.gaohongyu789.top

[Q68] 保存点
来源：http://uhu.shangyingyoupin.top

SAVEPOINT sp1;
来源：http://orh.yj20258888.top

ROLLBACK TO sp1;
来源：http://mlz.quarkkingdee.top

[Q69] 查看执行计划
来源：http://exz.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://unv.jqgufenzy.top

[Q70] 更新统计信息
来源：http://beb.zhoulong.xyz

ANALYZE TABLE users;
来源：http://kev.zycfv.cn

[Q71] 查看建表语句
来源：http://crr.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yvi.tarul.cn

[Q72] 查看索引
来源：http://iva.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://pbo.yj20258.top

[Q73] 查看表状态
来源：http://hxl.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ngm.redwolf501.top

[Q74] 强制使用索引
来源：http://fwd.ppjwa.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xvj.chenlongwang.top

[Q75] 日期格式化
来源：http://baw.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dgu.shanyushiyangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fxv.hnxiangtu.top

[Q76] 按天统计
来源：http://fre.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dwp.yfazqb.com

[Q77] 时间加减
来源：http://ndn.hnxiangtu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oiw.vqdsnc.cn

[Q78] 当前时间
来源：http://vbh.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nvn.svipenyu.cn

[Q79] 字符串拼接
来源：http://snd.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tgy.tarul.cn

[Q80] 字符串截取
来源：http://uxg.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://huv.0kj1m.cn

[Q81] 字符串替换
来源：http://vbk.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dgr.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://tjk.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://diz.sweek.top

[Q83] 大小写转换
来源：http://qhw.nanxuanxn.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mqi.guowangkeji.top

[Q84] 去除首尾空格
来源：http://wlu.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://tdl.feifeiyinyue.top

[Q85] 数值取整
来源：http://ulr.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rvh.yongpay.top

[Q86] 读取 JSON 字段
来源：http://upu.guowangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tfy.xuetiantiany.cn

[Q87] JSON 字段做条件
来源：http://nvd.zhijiandao.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://abm.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://bvt.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tkb.pengpengdd.cyou

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yrl.bbcook.cn

[Q89] 判断表是否存在
来源：http://abs.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xsx.iojbl.cn

[Q90] 生成序号列
来源：http://uso.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mxg.fzhhl.top

================================================================================
来源：http://fzf.zhengqikj.top

R. Bash 专题
来源：http://mza.shuidangran.top

================================================================================
来源：http://sga.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://znk.pengpengdd.cyou

#!/usr/bin/env bash
来源：http://qsy.havefunace.top

set -euo pipefail
来源：http://anu.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://xzl.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://gjy.fanxiaobao.xyz

[R03] 只读变量
来源：http://xom.yuanzhike.top

readonly PI=3.14
来源：http://hwx.shanyushiyangtech.top

[R04] 位置参数
来源：http://gjv.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://suj.bjfxy.top

[R05] 参数默认值
来源：http://fjz.guannengcc.top

name="${1:-default}"
来源：http://lml.zhixingplan.top

[R06] 判断命令是否存在
来源：http://ljb.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ato.feifeiyinyue.top

[R07] if 判断文件
来源：http://nmq.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jku.gotoacloud.top

[R08] 数值比较
来源：http://lep.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kxy.tanke756.top

[R09] 字符串比较
来源：http://gfs.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jgl.yuanzhike.top

[R10] 正则匹配
来源：http://wyk.jqgfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pja.yongpay.top

[R11] case 多分支
来源：http://ntj.52xcode.cn

case "$1" in
来源：http://rzt.bjfxy.top

start) echo "启动" ;;
来源：http://btv.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://rkj.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://flc.sweek.top

esac
来源：http://evw.vehdjk.com

[R12] for 遍历文件
来源：http://zpw.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://tpi.yangfankeji.com

[R13] for 计数循环
来源：http://mku.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://vvj.hywenlv.cn

[R14] C 风格 for
来源：http://rtn.yfazqb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kie.yonumen.top

[R15] while 逐行读文件
来源：http://fsp.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://til.sxryk.cn

[R16] until 等待条件
来源：http://dys.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rdo.52xcode.cn

[R17] 数组定义与取值
来源：http://mlq.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://zkf.cqqwz.cn

[R18] 遍历数组
来源：http://aqf.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rde.smart0.xyz

[R19] 数组长度
来源：http://rjj.nanxuanxn.top

echo "${#arr[@]}"
来源：http://rsi.yfazqb.com

[R20] 关联数组（字典）
来源：http://hsz.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xjc.wangdashe.top

[R21] 字符串长度
来源：http://bpi.fzhhl.top

echo "${#s}"
来源：http://ehi.zhixingplan.top

[R22] 截取子串
来源：http://uhd.gaohongyu789.top

echo "${s:0:5}"
来源：http://vvs.shuidangran.top

[R23] 字符串替换
来源：http://ych.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ryp.fzhhl.top

[R24] 大小写转换
来源：http://xsv.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://khx.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://bmv.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mem.yongpay.top

[R26] 命令替换
来源：http://jiu.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://upp.hnqzz.top

[R27] 算术展开
来源：http://gdy.wangdashe.top

echo $((1 + 2 * 3))
来源：http://rub.zhengqikj.top

[R28] 浮点运算
来源：http://rui.shanyushiyangtech.top

echo "scale=2; 10/3" | bc
来源：http://ipk.meibo888.top

[R29] 定义函数
来源：http://mkc.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fsm.hysaishi.cn

[R30] 函数返回状态码
来源：http://dag.fanxiaobao.xyz

f() { return 0; }; f || echo "失败了"
来源：http://gud.gaohongyu789.top

[R31] 局部变量
来源：http://qfh.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://lal.ydzc1.top

[R32] 参数个数校验
来源：http://gpq.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iww.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://xzx.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://juw.smart0.xyz

[R34] 退出时清理
来源：http://vtm.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://ivf.yj20258.top

[R35] 后台执行并等待
来源：http://ila.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kgj.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://msy.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fcm.zycfv.cn

[R37] 把输出赋给变量
来源：http://juq.vehdjk.com

files=$(ls -1)
来源：http://bjf.jinyuanbaomall.cn

[R38] 管道串联
来源：http://gvo.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://qsd.jqgufenzy.top

[R39] 重定向标准输出与错误
来源：http://zzx.xylfe.cn

cmd > out.log 2>&1
来源：http://jfp.ybcxt.top

[R40] 追加写日志
来源：http://cxr.0kj1m.cn

echo "log" >> out.log
来源：http://ehi.wangshuangyany.cn

[R41] 丢弃输出
来源：http://jel.yj202588.top

cmd >/dev/null 2>&1
来源：http://qig.chenzaomai.com

[R42] 输入重定向
来源：http://bke.dianchejie.cn

wc -l < a.txt
来源：http://oqj.zhengqikj.top

[R43] 按名字查找文件
来源：http://otx.cqqwz.cn

find . -name "*.log" -type f
来源：http://vop.yanxiufei.cn

[R44] 按修改时间查找
来源：http://rwg.ppjwa.cn

find . -mtime -7 -type f
来源：http://ntt.ydjk.org.cn

[R45] 批量删除
来源：http://zrf.fanxiaobao.xyz

find . -name "*.tmp" -delete
来源：http://pxu.bbcook.cn

[R46] 递归替换文件内容
来源：http://uar.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jsc.xinyue.icu

[R47] sed 单行替换
来源：http://wfx.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://kwi.yj20258.top

[R48] awk 取指定列
来源：http://ini.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://lmu.c1oappe.top

[R49] awk 带条件
来源：http://uyx.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gtq.mhx1999.top

[R50] awk 求和
来源：http://ewi.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://jhv.shuidangran.top

[R51] 排序去重取前几
来源：http://uyx.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://scz.ppjwa.cn

[R52] 统计行数
来源：http://hed.dianchejie.cn

wc -l a.txt
来源：http://qdm.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://zjp.dianchejie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ghq.tarul.cn

[R54] 比较两个文件
来源：http://job.xuanzx.com

diff a.txt b.txt
来源：http://kxk.xuanzx.com

[R55] 压缩与解压
来源：http://rwf.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zes.xuetiantiany.cn

[R56] 远程拷贝
来源：http://fne.jianghu66.top

scp file user@host:/path/
来源：http://gbj.ydzc1.top

[R57] 远程执行命令
来源：http://sdc.bjfxy.top

ssh user@host 'uptime'
来源：http://lmn.jinyuanbaomall.cn

[R58] 下载文件
来源：http://myw.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wax.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://vtd.ppjwa.cn


<!-- 参考信息 -->