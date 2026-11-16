代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://omp.smart0.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://juw.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kwg.ivvv.top

[Q15] 查询全部
来源：http://xje.jlsjyb.cn

SELECT * FROM users;
来源：http://lxv.cqqwz.cn

[Q16] 查询指定列
来源：http://hdp.xuanzx.com

SELECT id, name FROM users;
来源：http://pvm.cheryme.top

[Q17] 条件查询
来源：http://wnd.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ozu.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://irm.guannengcc.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kqs.zhijiandao.cn

[Q19] 范围查询
来源：http://pgk.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kpp.tarul.cn

[Q20] IN 列表
来源：http://pmv.jqgufenzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lce.ydjk.org.cn

[Q21] 空值判断
来源：http://uid.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fdi.jqgfzy.top

[Q22] 排序
来源：http://jjz.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pox.zdqjudy.top

[Q23] 分页
来源：http://new.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lvt.hnxiangtu.top

[Q24] 去重
来源：http://hdz.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://nqz.cucudq.cn

[Q25] 只取前 N 条
来源：http://zbo.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zuh.yj20258888.top

[Q26] 计数
来源：http://xxf.epnwcf.com

SELECT COUNT(*) FROM users;
来源：http://hfo.cdnleiting.top

[Q27] 条件计数
来源：http://omk.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qju.bbcook.cn

[Q28] 求和与平均
来源：http://ovb.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lse.redwolf501.top

[Q29] 最大最小值
来源：http://byg.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dvz.cqqwz.cn

[Q30] 分组统计
来源：http://mlz.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uta.meibo888.top

[Q31] 分组后过滤
来源：http://lqo.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jiw.aizwys.cn

[Q32] 分组拼接字符串
来源：http://xms.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wnr.c1oappe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cnw.tianlin.xyz

[Q33] 多列分组
来源：http://bbk.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rgu.xinyue.icu

[Q34] 每组取第一条
来源：http://usb.guannengcc.top

SELECT * FROM (
来源：http://xcm.52xcode.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://puz.jinqigfzy.top

) t WHERE rn = 1;
来源：http://zow.hesvh.cn

[Q35] 内连接
来源：http://sqn.yj20258.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hlj.yj20258888.top

[Q36] 左连接
来源：http://irf.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hco.quarkkingdee.top

[Q37] 右连接
来源：http://dkt.nanxuanxn.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://foa.sysykeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://eyc.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zsj.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://nvj.yongpay.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zcf.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mqv.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vhz.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nwo.yuxming.cn

[Q41] 多表连接
来源：http://ofn.aizwys.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kem.guowangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://jvm.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://mhd.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://mpp.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://qkx.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://she.bjfxy.top

[Q43] 标量子查询
来源：http://rkq.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bji.hnqzz.top

[Q44] IN 子查询
来源：http://kaj.yuanzhike.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hhe.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://bvp.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://djg.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://uwp.zhongyouzk.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://poa.zhengqikj.top

[Q47] 与平均值比较
来源：http://vdo.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vha.aizwys.cn

[Q48] CTE 公用表表达式
来源：http://aqx.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wpl.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://fie.yonumen.top

[Q49] 更新单行
来源：http://lnb.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jsb.zhiwuduotai.top

[Q50] 批量更新
来源：http://lch.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nld.sxryk.cn

[Q51] 用子查询更新
来源：http://nqz.vehdjk.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://abk.fehbvm.com

[Q52] 删除指定行
来源：http://zof.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://gau.quarkkingdee.top

[Q53] 按条件删除
来源：http://cfe.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tts.shanyushiyangtech.top

[Q54] 清空表
来源：http://fcn.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://ego.redwolf501.top

[Q55] 排名（并列占位）
来源：http://nig.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bkf.zdqjudy.top

[Q56] 密集排名（并列不占位）
来源：http://eav.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yhi.redwolf501.top

[Q57] 行号
来源：http://guv.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rck.hnqzz.top

[Q58] 累计求和
来源：http://cjt.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wpv.52xcode.cn

[Q59] 分组内累计
来源：http://bgf.tanke756.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zdq.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://kos.dashuyun.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gyc.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eqo.yonumen.top

[Q61] 移动平均
来源：http://inr.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ztp.xuetiantiany.cn

[Q62] 分组占比
来源：http://mxu.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yjl.tarul.cn

[Q63] 开启事务
来源：http://nqc.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dau.ybcxt.top

[Q64] 提交事务
来源：http://btq.ehwqpu.com

COMMIT;
来源：http://nas.yongpay.top

[Q65] 回滚事务
来源：http://qln.andypj.xyz

ROLLBACK;
来源：http://tbu.tianlin.xyz

[Q66] 行锁查询
来源：http://tmg.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://txw.nanxuanxn.top

[Q67] 设置隔离级别
来源：http://har.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nnf.ydzc1.top

[Q68] 保存点
来源：http://cog.316326.xyz

SAVEPOINT sp1;
来源：http://ygz.fktsv.cn

ROLLBACK TO sp1;
来源：http://inb.nanxinkj.top

[Q69] 查看执行计划
来源：http://hba.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wcp.hnqzz.top

[Q70] 更新统计信息
来源：http://dsp.pengpengdd.cyou

ANALYZE TABLE users;
来源：http://yhn.sjlbkw.cn

[Q71] 查看建表语句
来源：http://zqw.cheryme.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ksk.aibaodan.cn

[Q72] 查看索引
来源：http://opx.zdqjudy.top

SHOW INDEX FROM users;
来源：http://mdf.ehwqpu.com

[Q73] 查看表状态
来源：http://vka.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xnk.dianchejie.cn

[Q74] 强制使用索引
来源：http://ydq.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hlo.pycfn.com

[Q75] 日期格式化
来源：http://rqt.yfazqb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ckl.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bgj.vehdjk.com

[Q76] 按天统计
来源：http://zkh.meibo888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sln.pengpengdd.cyou

[Q77] 时间加减
来源：http://wyx.chenjidiqi.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ayp.cdnleiting.top

[Q78] 当前时间
来源：http://xhn.zdqjudy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://drv.guowangkeji.top

[Q79] 字符串拼接
来源：http://gqq.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ppb.guannengcc.top

[Q80] 字符串截取
来源：http://xvg.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rjq.gzhubu.top

[Q81] 字符串替换
来源：http://xvw.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://abv.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://tuc.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fsb.xziqi.cn

[Q83] 大小写转换
来源：http://aku.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jgj.cdnleiting.top

[Q84] 去除首尾空格
来源：http://ffv.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://ydr.sufxvd.cn

[Q85] 数值取整
来源：http://tvi.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ygk.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://vai.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jut.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://lqa.shanyushiyangtech.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aif.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://gcj.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yvv.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tze.gaohongyu789.top

[Q89] 判断表是否存在
来源：http://gur.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rvq.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://mmu.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aha.cdnleiting.top

================================================================================
来源：http://pgi.nanxuanxn.top

R. Bash 专题
来源：http://iqp.zycfv.cn

================================================================================
来源：http://mkf.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://gzj.ehwqpu.com

#!/usr/bin/env bash
来源：http://hgi.hysaishi.cn

set -euo pipefail
来源：http://rua.ehwqpu.com

[R02] 变量赋值与使用
来源：http://kzh.smart0.xyz

name="Tom"; echo "$name"
来源：http://cit.sjlbkw.cn

[R03] 只读变量
来源：http://ttc.fengsongda.top

readonly PI=3.14
来源：http://ssi.wangshuangyany.cn

[R04] 位置参数
来源：http://dyo.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ppn.aibaodan.cn

[R05] 参数默认值
来源：http://nbd.zhaomingkeji.xyz

name="${1:-default}"
来源：http://dtb.yangfankeji.com

[R06] 判断命令是否存在
来源：http://tgj.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://efn.mhx1999.top

[R07] if 判断文件
来源：http://tqu.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cwz.hysaishi.cn

[R08] 数值比较
来源：http://bav.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jan.nanxinkj.top

[R09] 字符串比较
来源：http://jnc.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zgt.yangfankeji.com

[R10] 正则匹配
来源：http://sjg.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xoj.hnxiangtu.top

[R11] case 多分支
来源：http://sbu.xziqi.cn

case "$1" in
来源：http://phz.andypj.xyz

start) echo "启动" ;;
来源：http://swh.fehbvm.com

stop)  echo "停止" ;;
来源：http://jcj.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://exy.zhaomingkeji.xyz

esac
来源：http://ius.xuanzx.com

[R12] for 遍历文件
来源：http://vuf.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://uhb.ppjwa.cn

[R13] for 计数循环
来源：http://qth.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://vde.pycfn.com

[R14] C 风格 for
来源：http://lit.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vmb.dianchejie.cn

[R15] while 逐行读文件
来源：http://ehe.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iei.feifeiyinyue.top

[R16] until 等待条件
来源：http://dik.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wsp.yvedp.cn

[R17] 数组定义与取值
来源：http://pga.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vap.hysaishi.cn

[R18] 遍历数组
来源：http://asa.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ukq.smart0.xyz

[R19] 数组长度
来源：http://rey.gzhubu.top

echo "${#arr[@]}"
来源：http://xsq.yueranfly.top

[R20] 关联数组（字典）
来源：http://xok.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ysf.tianlin.xyz

[R21] 字符串长度
来源：http://czw.gaohongyu789.top

echo "${#s}"
来源：http://wkz.wangdashe.top

[R22] 截取子串
来源：http://izn.52xcode.cn

echo "${s:0:5}"
来源：http://ufw.nanxinkj.top

[R23] 字符串替换
来源：http://atf.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qlq.jinqigufen.top

[R24] 大小写转换
来源：http://ygg.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://xfe.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://run.chenzaomai.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://jcd.fzhhl.top

[R26] 命令替换
来源：http://roj.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://ssv.xuetiantiany.cn

[R27] 算术展开
来源：http://pfl.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://fjm.jianghu66.top

[R28] 浮点运算
来源：http://gyh.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://ivd.wangdashe.top

[R29] 定义函数
来源：http://qmf.hfpthk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://isi.feifeiyinyue.top

[R30] 函数返回状态码
来源：http://jxs.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://fht.quarkkingdee.top

[R31] 局部变量
来源：http://elz.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://pec.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://fbs.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qay.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://cls.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dtq.ydjk.org.cn

[R34] 退出时清理
来源：http://udn.fanxiaobao.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ldu.fzhhl.top

[R35] 后台执行并等待
来源：http://uvm.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://nla.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://iax.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mpm.zycfv.cn

[R37] 把输出赋给变量
来源：http://lui.ppjwa.cn

files=$(ls -1)
来源：http://jfp.ivvv.top

[R38] 管道串联
来源：http://qwf.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://kkl.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://rvg.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://tqx.guannengcc.top

[R40] 追加写日志
来源：http://jro.cheryme.top

echo "log" >> out.log
来源：http://kfr.fehbvm.com

[R41] 丢弃输出
来源：http://veq.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://wic.yuanzhike.top

[R42] 输入重定向
来源：http://eso.nanxinkj.top

wc -l < a.txt
来源：http://llw.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://pef.yanxiufei.cn

find . -name "*.log" -type f
来源：http://itf.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://cpj.yfazqb.com

find . -mtime -7 -type f
来源：http://rrf.jinghuilouyu.cn

[R45] 批量删除
来源：http://lmy.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://ftl.meibo888.top

[R46] 递归替换文件内容
来源：http://vko.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zcj.fehbvm.com

[R47] sed 单行替换
来源：http://kvv.tian-w.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pgk.yuanzhike.top

[R48] awk 取指定列
来源：http://kgl.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://jqg.pycfn.com

[R49] awk 带条件
来源：http://orj.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dpb.zhongyouzk.top

[R50] awk 求和
来源：http://vjt.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://dpy.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://omx.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lkk.bjfxy.top

[R52] 统计行数
来源：http://ciu.snrcjt.cn

wc -l a.txt
来源：http://ysw.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://sil.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ojk.jinqigfzy.top

[R54] 比较两个文件
来源：http://nng.0kj1m.cn

diff a.txt b.txt
来源：http://cjk.redwolf501.top

[R55] 压缩与解压
来源：http://sob.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://awe.ywan-chungtsiang.top

[R56] 远程拷贝
来源：http://tmg.vqdsnc.cn

scp file user@host:/path/
来源：http://ktv.dashuyun.cn

[R57] 远程执行命令
来源：http://ggv.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://fgs.sysykeji.top

[R58] 下载文件
来源：http://qxf.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bne.wangshuangyany.cn

[R59] 发 POST JSON
来源：http://rme.nanxuanxn.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://whv.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://rth.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nox.xinyue.icu

[R61] 磁盘占用
来源：http://njo.yvedp.cn

df -h;  du -sh *
来源：http://lpc.ydzc1.top

[R62] 找最占空间的文件
来源：http://psy.fzhhl.top

du -ah . | sort -rh | head -10
来源：http://uiw.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://ikw.kuanghao11.cn


<!-- 参考信息 -->