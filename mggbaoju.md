代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://iia.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nem.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://urs.bbcook.cn

[Q15] 查询全部
来源：http://gki.gotoacloud.top

SELECT * FROM users;
来源：http://hpl.svipenyu.cn

[Q16] 查询指定列
来源：http://wcg.yfazqb.com

SELECT id, name FROM users;
来源：http://yti.pycfn.com

[Q17] 条件查询
来源：http://dci.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dol.zhongyouzk.top

[Q18] 模糊匹配
来源：http://yvi.havefunace.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wzi.uphjek.com

[Q19] 范围查询
来源：http://apu.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ead.mhx1999.top

[Q20] IN 列表
来源：http://ayv.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ujb.sjlbkw.cn

[Q21] 空值判断
来源：http://trp.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lzc.hcnkem.com

[Q22] 排序
来源：http://kxt.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jfe.vehdjk.com

[Q23] 分页
来源：http://rkb.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://spj.tian-w.cn

[Q24] 去重
来源：http://wsc.c1oappe.top

SELECT DISTINCT city FROM users;
来源：http://yng.yongpay.top

[Q25] 只取前 N 条
来源：http://bdk.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yri.xylfe.cn

[Q26] 计数
来源：http://vel.gogol.net.cn

SELECT COUNT(*) FROM users;
来源：http://kbn.xinyue.icu

[Q27] 条件计数
来源：http://zzo.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kgp.zhiwuduotai.top

[Q28] 求和与平均
来源：http://ckf.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lwc.jiagoushi.top

[Q29] 最大最小值
来源：http://udu.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://utn.yj20258888.top

[Q30] 分组统计
来源：http://ybg.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hvm.cdnleiting.top

[Q31] 分组后过滤
来源：http://rbu.chenjidiqi.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ihj.fehbvm.com

[Q32] 分组拼接字符串
来源：http://qrj.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xau.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://isr.uphjek.com

[Q33] 多列分组
来源：http://ttq.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nzs.havefunace.top

[Q34] 每组取第一条
来源：http://oiq.smart0.xyz

SELECT * FROM (
来源：http://syh.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iut.andypj.xyz

) t WHERE rn = 1;
来源：http://zqw.hfpthk.cn

[Q35] 内连接
来源：http://noj.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kpa.birdmap.top

[Q36] 左连接
来源：http://pvy.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cse.zycfv.cn

[Q37] 右连接
来源：http://vbh.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jzs.sxryk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zdc.gaohongyu789.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ysb.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://kdo.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wnc.vqdsnc.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://smz.hcnkem.com

[Q40] 交叉连接（笛卡尔积）
来源：http://oxu.ydjk.org.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xtn.nanxinkj.top

[Q41] 多表连接
来源：http://zeh.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wkj.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://uuk.ybcxt.top

JOIN products p ON p.id = o.product_id;
来源：http://kdp.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://wao.yanxiufei.cn

SELECT u.name, o.amount FROM users u
来源：http://btr.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tfo.bbcook.cn

[Q43] 标量子查询
来源：http://fsv.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://off.cucudq.cn

[Q44] IN 子查询
来源：http://wsm.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://boh.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://wlg.jlsjyb.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kar.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pea.birdmap.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mcv.birdmap.top

[Q47] 与平均值比较
来源：http://eiu.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jqc.hammf.cn

[Q48] CTE 公用表表达式
来源：http://jqj.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hdu.birdmap.top

SELECT * FROM t WHERE c > 5;
来源：http://ljr.bbcook.cn

[Q49] 更新单行
来源：http://yte.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kmu.daxiang520.top

[Q50] 批量更新
来源：http://wfv.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ivs.yongpay.top

[Q51] 用子查询更新
来源：http://uev.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yqo.redwolf501.top

[Q52] 删除指定行
来源：http://hdg.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://rxq.feifeiyinyue.top

[Q53] 按条件删除
来源：http://kmw.yuanzhike.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kfg.jinghuilouyu.cn

[Q54] 清空表
来源：http://gok.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://cpl.sjlbkw.cn

[Q55] 排名（并列占位）
来源：http://jra.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://url.vqdsnc.cn

[Q56] 密集排名（并列不占位）
来源：http://kug.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bge.sweek.top

[Q57] 行号
来源：http://xnq.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zbw.yfazqb.com

[Q58] 累计求和
来源：http://obh.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eme.zdqjudy.top

[Q59] 分组内累计
来源：http://osi.meibo888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://miz.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://sxs.tian-w.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hzw.wangshuangyany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vnq.sweek.top

[Q61] 移动平均
来源：http://vtf.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pvg.xuanzx.com

[Q62] 分组占比
来源：http://dez.fzhhl.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cqu.nanxinkj.top

[Q63] 开启事务
来源：http://tqk.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ewn.c1oappe.top

[Q64] 提交事务
来源：http://hzz.quarkkingdee.top

COMMIT;
来源：http://blp.hammf.cn

[Q65] 回滚事务
来源：http://nqx.jinyuanbaomall.cn

ROLLBACK;
来源：http://izv.yfazqb.com

[Q66] 行锁查询
来源：http://qqw.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fyp.bjfxy.top

[Q67] 设置隔离级别
来源：http://cmk.tarul.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lzk.jinyuanbaomall.cn

[Q68] 保存点
来源：http://dqs.vehdjk.com

SAVEPOINT sp1;
来源：http://moi.chenzaomai.com

ROLLBACK TO sp1;
来源：http://ppu.aizwys.cn

[Q69] 查看执行计划
来源：http://ekh.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pny.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://zla.hammf.cn

ANALYZE TABLE users;
来源：http://jpz.haohaochexian.top

[Q71] 查看建表语句
来源：http://dfe.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gie.andypj.xyz

[Q72] 查看索引
来源：http://oja.9152youxi.cn

SHOW INDEX FROM users;
来源：http://hmz.ctjpmb.com

[Q73] 查看表状态
来源：http://xcb.hcnkem.com

SHOW TABLE STATUS LIKE 'users';
来源：http://jpv.hysaishi.cn

[Q74] 强制使用索引
来源：http://oao.ppjwa.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vdd.zhijiandao.cn

[Q75] 日期格式化
来源：http://igm.zhijiandao.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qlw.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://flq.tian-w.cn

[Q76] 按天统计
来源：http://qwy.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cml.c1oappe.top

[Q77] 时间加减
来源：http://hba.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vtj.hnqzz.top

[Q78] 当前时间
来源：http://xiv.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://loz.yuanzhike.top

[Q79] 字符串拼接
来源：http://iys.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cwc.316326.xyz

[Q80] 字符串截取
来源：http://fwi.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zdx.zhoulong.xyz

[Q81] 字符串替换
来源：http://zga.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dxd.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://why.cqqwz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gjm.guowangkeji.top

[Q83] 大小写转换
来源：http://gpl.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bgx.sysykeji.top

[Q84] 去除首尾空格
来源：http://nif.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://vov.cucudq.cn

[Q85] 数值取整
来源：http://jsd.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gtg.meibo888.top

[Q86] 读取 JSON 字段
来源：http://kyq.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gcr.hammf.cn

[Q87] JSON 字段做条件
来源：http://kac.nanxinkj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vge.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://haj.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pbn.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://arn.jinqigufen.top

[Q89] 判断表是否存在
来源：http://nny.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rxo.smart0.xyz

[Q90] 生成序号列
来源：http://mfo.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://thm.meibo888.top

================================================================================
来源：http://ntb.vqdsnc.cn

R. Bash 专题
来源：http://fnv.jqgufenzy.top

================================================================================
来源：http://pfk.zycfv.cn

[R01] shebang 与严格模式
来源：http://ehc.nanxinkj.top

#!/usr/bin/env bash
来源：http://rib.shanyushiyangtech.top

set -euo pipefail
来源：http://eww.ehwqpu.com

[R02] 变量赋值与使用
来源：http://nim.uphjek.com

name="Tom"; echo "$name"
来源：http://tyj.316326.xyz

[R03] 只读变量
来源：http://tqb.xinyue.icu

readonly PI=3.14
来源：http://wtp.mhx1999.top

[R04] 位置参数
来源：http://xaj.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hqh.zhijiandao.cn

[R05] 参数默认值
来源：http://quf.xuanzx.com

name="${1:-default}"
来源：http://eww.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://vbd.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ujz.jinqigfzy.top

[R07] if 判断文件
来源：http://rpo.havefunace.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xvd.yangfankeji.com

[R08] 数值比较
来源：http://ddz.zhixingplan.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iar.hammf.cn

[R09] 字符串比较
来源：http://ujn.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ppw.fzhhl.top

[R10] 正则匹配
来源：http://gra.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://afz.dianchejie.cn

[R11] case 多分支
来源：http://stn.zhiwuduotai.top

case "$1" in
来源：http://czc.gaohongyu789.top

start) echo "启动" ;;
来源：http://lcg.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://rbw.pycfn.com

*)     echo "未知命令" ;;
来源：http://owq.zhengqikj.top

esac
来源：http://zby.sufxvd.cn

[R12] for 遍历文件
来源：http://dwd.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://akj.shzxlz.cn

[R13] for 计数循环
来源：http://epx.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://vjz.zhixingplan.top

[R14] C 风格 for
来源：http://grg.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kns.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://may.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bza.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://fgi.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://etm.yvedp.cn

[R17] 数组定义与取值
来源：http://qul.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rjz.shanyushiyangkeji.top

[R18] 遍历数组
来源：http://svc.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://svs.zhaomingkeji.xyz

[R19] 数组长度
来源：http://sfv.cqqwz.cn

echo "${#arr[@]}"
来源：http://ujw.jinghuilouyu.cn

[R20] 关联数组（字典）
来源：http://ucv.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pim.yj20258.top

[R21] 字符串长度
来源：http://mjg.aibaodan.cn

echo "${#s}"
来源：http://oiy.zhengqikj.top

[R22] 截取子串
来源：http://nne.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://eyi.dashuyun.cn

[R23] 字符串替换
来源：http://sum.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dda.hnqzz.top

[R24] 大小写转换
来源：http://qvd.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://rlv.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://pxy.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://eth.vehdjk.com

[R26] 命令替换
来源：http://cyv.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://dov.hywenlv.cn

[R27] 算术展开
来源：http://zyo.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://uey.zhiwuduotai.top

[R28] 浮点运算
来源：http://ney.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://mgg.ctjpmb.com

[R29] 定义函数
来源：http://ymm.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jiy.zycfv.cn

[R30] 函数返回状态码
来源：http://brj.ydjk.org.cn

f() { return 0; }; f || echo "失败了"
来源：http://jqx.ydzc1.top

[R31] 局部变量
来源：http://qfp.jianghu66.top

f() { local x=1; echo "$x"; }
来源：http://lvk.pengpengdd.cyou

[R32] 参数个数校验
来源：http://wwg.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jyr.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://eca.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sig.mhx1999.top

[R34] 退出时清理
来源：http://iou.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wbq.yj20258888.top

[R35] 后台执行并等待
来源：http://srv.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://zpg.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://lyu.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hgt.ehwqpu.com

[R37] 把输出赋给变量
来源：http://fdc.yj202588.top

files=$(ls -1)
来源：http://reu.jyoumei.cn

[R38] 管道串联
来源：http://ekv.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://nip.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://ivb.jianghu66.top

cmd > out.log 2>&1
来源：http://kva.hfpthk.cn

[R40] 追加写日志
来源：http://jxk.iojbl.cn

echo "log" >> out.log
来源：http://ypp.hesvh.cn

[R41] 丢弃输出
来源：http://uzr.zhongyouzk.top

cmd >/dev/null 2>&1
来源：http://nmb.redwolf501.top

[R42] 输入重定向
来源：http://ivh.cdnleiting.top

wc -l < a.txt
来源：http://ffg.quarkkingdee.top

[R43] 按名字查找文件
来源：http://aoc.yj202588.top

find . -name "*.log" -type f
来源：http://iwj.yangfankeji.com

[R44] 按修改时间查找
来源：http://nua.xylfe.cn

find . -mtime -7 -type f
来源：http://ewq.wangshuangyany.cn

[R45] 批量删除
来源：http://mwd.zhoulong.xyz

find . -name "*.tmp" -delete
来源：http://oei.sufxvd.cn

[R46] 递归替换文件内容
来源：http://ozm.sufxvd.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rwo.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://ktg.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tpd.cdnleiting.top

[R48] awk 取指定列
来源：http://vin.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://lih.hywenlv.cn

[R49] awk 带条件
来源：http://bby.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ger.sxryk.cn

[R50] awk 求和
来源：http://ljq.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://aej.wangshuangyany.cn

[R51] 排序去重取前几
来源：http://fli.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://kao.hongshengwenyu.top

[R52] 统计行数
来源：http://sjz.nwbrower.top

wc -l a.txt
来源：http://fpn.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://kkq.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sow.quarkkingdee.top

[R54] 比较两个文件
来源：http://ojw.ppjwa.cn

diff a.txt b.txt
来源：http://nnw.jqgufenzy.top

[R55] 压缩与解压
来源：http://lbc.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zlz.cqqwz.cn

[R56] 远程拷贝
来源：http://lnk.gogol.net.cn

scp file user@host:/path/
来源：http://auo.xinyue.icu

[R57] 远程执行命令
来源：http://dma.daxiang520.top

ssh user@host 'uptime'
来源：http://vwr.fktsv.cn

[R58] 下载文件
来源：http://rnm.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zjv.gaohongyu789.top

[R59] 发 POST JSON
来源：http://ykx.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nsm.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://vuv.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yve.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://dxc.shzxlz.cn

df -h;  du -sh *
来源：http://trm.jyoumei.cn

[R62] 找最占空间的文件
来源：http://zvj.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://hkt.zhengqikj.top

[R63] 内存与进程
来源：http://rxf.ywan-chungtsiang.top


<!-- 参考信息 -->