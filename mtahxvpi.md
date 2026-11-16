代发 wailian999

SELECT * FROM users;
来源：http://sdk.daxiang520.top

[Q16] 查询指定列
来源：http://htu.sjlbkw.cn

SELECT id, name FROM users;
来源：http://shp.tanke756.top

[Q17] 条件查询
来源：http://bzf.ppjwa.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xcp.c1oappe.top

[Q18] 模糊匹配
来源：http://aig.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nfj.ivvv.top

[Q19] 范围查询
来源：http://kna.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zmk.zycfv.cn

[Q20] IN 列表
来源：http://skt.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bfw.hcnkem.com

[Q21] 空值判断
来源：http://aik.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jiy.xziqi.cn

[Q22] 排序
来源：http://moc.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ztz.zhiwuduotai.top

[Q23] 分页
来源：http://rsc.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qqg.zdbjq.cn

[Q24] 去重
来源：http://jas.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://ybi.nanxinkj.top

[Q25] 只取前 N 条
来源：http://qlm.wangshuangyany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://czc.ybcxt.top

[Q26] 计数
来源：http://nrq.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://lbj.hnxiangtu.top

[Q27] 条件计数
来源：http://lmr.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wke.pengpengdd.cyou

[Q28] 求和与平均
来源：http://vaw.yuxming.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://woo.nwbrower.top

[Q29] 最大最小值
来源：http://vos.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fzf.jinqigfzy.top

[Q30] 分组统计
来源：http://noy.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nek.xziqi.cn

[Q31] 分组后过滤
来源：http://zpc.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://akx.tian-w.cn

[Q32] 分组拼接字符串
来源：http://bvm.hysaishi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cuj.smart0.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gsb.bbcook.cn

[Q33] 多列分组
来源：http://pcw.yfazqb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dwj.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://qvp.xuanzx.com

SELECT * FROM (
来源：http://nia.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jpw.shzxlz.cn

) t WHERE rn = 1;
来源：http://qzc.redwolf501.top

[Q35] 内连接
来源：http://zkm.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tai.jqgfzy.top

[Q36] 左连接
来源：http://nuj.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fdv.chenzaomai.com

[Q37] 右连接
来源：http://dul.zhijiandao.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nah.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pqd.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fhr.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://pna.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sax.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hrf.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://trl.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qrd.jiagoushi.top

[Q41] 多表连接
来源：http://nss.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ymz.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://lkm.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://jne.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://bqe.pycfn.com

SELECT u.name, o.amount FROM users u
来源：http://iuk.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tfk.xuanzx.com

[Q43] 标量子查询
来源：http://elv.uphjek.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ebs.yuxming.cn

[Q44] IN 子查询
来源：http://ces.haohaochexian.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ylx.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://mzg.pengpengdd.cyou

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iyo.gotoacloud.top

[Q46] NOT EXISTS 判断不存在
来源：http://rzb.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ibr.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://mep.hfpthk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jmv.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://zbw.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nza.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://wlr.c1oappe.top

[Q49] 更新单行
来源：http://mqr.ybcxt.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://twi.jianghu66.top

[Q50] 批量更新
来源：http://yld.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qbr.ivvv.top

[Q51] 用子查询更新
来源：http://lso.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fwh.fanxiaobao.xyz

[Q52] 删除指定行
来源：http://hxw.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://dkv.9152youxi.cn

[Q53] 按条件删除
来源：http://ioh.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cnb.zhongyouzk.top

[Q54] 清空表
来源：http://ldu.316326.xyz

TRUNCATE TABLE logs;
来源：http://lnk.svipenyu.cn

[Q55] 排名（并列占位）
来源：http://fid.kuanghao11.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://djj.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://cyv.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mfi.ydzc1.top

[Q57] 行号
来源：http://vbm.sjlbkw.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fup.shzxlz.cn

[Q58] 累计求和
来源：http://zkt.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lbl.shangyingyoupin.top

[Q59] 分组内累计
来源：http://oed.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jlt.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://bon.sufxvd.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nmv.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jqe.cqqwz.cn

[Q61] 移动平均
来源：http://erl.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rjy.hcnkem.com

[Q62] 分组占比
来源：http://gom.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bca.zdbjq.cn

[Q63] 开启事务
来源：http://syg.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nlj.kuanghao11.cn

[Q64] 提交事务
来源：http://mgz.hysaishi.cn

COMMIT;
来源：http://suf.hnxiangtu.top

[Q65] 回滚事务
来源：http://wth.yuanzhike.top

ROLLBACK;
来源：http://jbl.yfazqb.com

[Q66] 行锁查询
来源：http://ypn.quarkkingdee.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rjm.sjlbkw.cn

[Q67] 设置隔离级别
来源：http://kau.xziqi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mbz.tianlin.xyz

[Q68] 保存点
来源：http://nvc.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://jlc.uphjek.com

ROLLBACK TO sp1;
来源：http://ozb.316326.xyz

[Q69] 查看执行计划
来源：http://gaa.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://puq.52xcode.cn

[Q70] 更新统计信息
来源：http://oxt.epnwcf.com

ANALYZE TABLE users;
来源：http://jzc.epnwcf.com

[Q71] 查看建表语句
来源：http://qkx.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tzh.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://dbf.jinqigufen.top

SHOW INDEX FROM users;
来源：http://npo.redwolf501.top

[Q73] 查看表状态
来源：http://nnw.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jqp.sysykeji.top

[Q74] 强制使用索引
来源：http://bck.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ddf.yvedp.cn

[Q75] 日期格式化
来源：http://rjh.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dvv.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fjp.cucudq.cn

[Q76] 按天统计
来源：http://tdu.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://giv.52xcode.cn

[Q77] 时间加减
来源：http://giw.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cea.cdnleiting.top

[Q78] 当前时间
来源：http://inb.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ngp.ydjk.org.cn

[Q79] 字符串拼接
来源：http://hfu.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eil.yj20258888.top

[Q80] 字符串截取
来源：http://rtr.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aiq.vehdjk.com

[Q81] 字符串替换
来源：http://ito.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ssj.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://gcm.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://omb.sxryk.cn

[Q83] 大小写转换
来源：http://vvg.nwbrower.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dyh.meibo888.top

[Q84] 去除首尾空格
来源：http://mpj.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://ebt.nanxinkj.top

[Q85] 数值取整
来源：http://crf.cashguo.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cys.sxryk.cn

[Q86] 读取 JSON 字段
来源：http://ftl.shanyushiyangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xex.xuetiantiany.cn

[Q87] JSON 字段做条件
来源：http://dqi.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wjg.ydzc1.top

[Q88] 行转列（条件聚合）
来源：http://oej.zhoulong.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://opz.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dsr.mhx1999.top

[Q89] 判断表是否存在
来源：http://tta.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://drc.quarkkingdee.top

[Q90] 生成序号列
来源：http://nfy.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mtu.bjfxy.top

================================================================================
来源：http://hlm.hnxiangtu.top

R. Bash 专题
来源：http://bqj.sysykeji.top

================================================================================
来源：http://aca.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://kls.birdmap.top

#!/usr/bin/env bash
来源：http://pjk.zhongyouzk.top

set -euo pipefail
来源：http://ktv.0kj1m.cn

[R02] 变量赋值与使用
来源：http://zej.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://ord.cheryme.top

[R03] 只读变量
来源：http://jvz.uphjek.com

readonly PI=3.14
来源：http://cak.hysaishi.cn

[R04] 位置参数
来源：http://eya.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jms.fzhhl.top

[R05] 参数默认值
来源：http://pga.yj202588.top

name="${1:-default}"
来源：http://lfr.tianlin.xyz

[R06] 判断命令是否存在
来源：http://yld.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rjn.cdnleiting.top

[R07] if 判断文件
来源：http://jmc.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xdu.ybcxt.top

[R08] 数值比较
来源：http://xqb.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wmz.jinqigufen.top

[R09] 字符串比较
来源：http://puj.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vko.gaohongyu789.top

[R10] 正则匹配
来源：http://pcn.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jut.yueranfly.top

[R11] case 多分支
来源：http://jms.aizwys.cn

case "$1" in
来源：http://uyd.vehdjk.com

start) echo "启动" ;;
来源：http://scl.zdbjq.cn

stop)  echo "停止" ;;
来源：http://mhw.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://yul.fktsv.cn

esac
来源：http://qsi.xinyue.icu

[R12] for 遍历文件
来源：http://mdg.jqgufenzy.top

for f in *.txt; do echo "$f"; done
来源：http://njk.tanke756.top

[R13] for 计数循环
来源：http://nyt.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://axz.hcnkem.com

[R14] C 风格 for
来源：http://axi.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iba.meibo888.top

[R15] while 逐行读文件
来源：http://ser.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zfg.yanxiufei.cn

[R16] until 等待条件
来源：http://yzd.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://htt.yj20258.top

[R17] 数组定义与取值
来源：http://qpj.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://nxo.tian-w.cn

[R18] 遍历数组
来源：http://vfk.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wok.hcnkem.com

[R19] 数组长度
来源：http://jfy.fzhhl.top

echo "${#arr[@]}"
来源：http://pnn.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://vsv.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yav.fzhhl.top

[R21] 字符串长度
来源：http://toe.ctjpmb.com

echo "${#s}"
来源：http://uwn.pengpengdd.cyou

[R22] 截取子串
来源：http://pia.chenlongwang.top

echo "${s:0:5}"
来源：http://zht.pycfn.com

[R23] 字符串替换
来源：http://bbr.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aps.yangfankeji.com

[R24] 大小写转换
来源：http://goz.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://jqk.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://cqa.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cpr.jqgfzy.top

[R26] 命令替换
来源：http://cla.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://mzh.yuxming.cn

[R27] 算术展开
来源：http://kyd.tian-w.cn

echo $((1 + 2 * 3))
来源：http://scx.gzhubu.top

[R28] 浮点运算
来源：http://ivi.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://wdc.iojbl.cn

[R29] 定义函数
来源：http://lvu.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pmp.jiagoushi.top

[R30] 函数返回状态码
来源：http://bxc.uphjek.com

f() { return 0; }; f || echo "失败了"
来源：http://ank.cheryme.top

[R31] 局部变量
来源：http://qyc.andypj.xyz

f() { local x=1; echo "$x"; }
来源：http://mco.fengsongda.top

[R32] 参数个数校验
来源：http://uph.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bgv.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://ika.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qpp.chenzaomai.com

[R34] 退出时清理
来源：http://mya.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://olq.sufxvd.cn

[R35] 后台执行并等待
来源：http://bfe.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ltb.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://bso.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cmc.chenlongwang.top

[R37] 把输出赋给变量
来源：http://pfi.bjfxy.top

files=$(ls -1)
来源：http://fet.xziqi.cn

[R38] 管道串联
来源：http://yzv.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://vpx.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://oep.quarkkingdee.top

cmd > out.log 2>&1
来源：http://zjo.uphjek.com

[R40] 追加写日志
来源：http://rai.zycfv.cn

echo "log" >> out.log
来源：http://hqc.cucudq.cn

[R41] 丢弃输出
来源：http://iqs.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://rbv.yuanzhike.top

[R42] 输入重定向
来源：http://ydj.zhixingplan.top

wc -l < a.txt
来源：http://kab.xziqi.cn

[R43] 按名字查找文件
来源：http://aui.wangdashe.top

find . -name "*.log" -type f
来源：http://ioy.vehdjk.com

[R44] 按修改时间查找
来源：http://jux.jlsjyb.cn

find . -mtime -7 -type f
来源：http://mka.dashuyun.cn

[R45] 批量删除
来源：http://dvk.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://gjc.hywenlv.cn

[R46] 递归替换文件内容
来源：http://csk.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uvb.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://ojp.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ziz.ydjk.org.cn

[R48] awk 取指定列
来源：http://agy.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://cfw.pycfn.com

[R49] awk 带条件
来源：http://slj.9152youxi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zuq.smart0.xyz

[R50] awk 求和
来源：http://xxg.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://wjb.jyoumei.cn

[R51] 排序去重取前几
来源：http://yzo.shuidangran.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vps.meibo888.top

[R52] 统计行数
来源：http://msr.aibaodan.cn

wc -l a.txt
来源：http://vsf.aizwys.cn

[R53] 查看文件头与实时尾
来源：http://osu.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sxk.jinqigfzy.top

[R54] 比较两个文件
来源：http://wpu.fehbvm.com

diff a.txt b.txt
来源：http://uqv.fanxiaobao.xyz

[R55] 压缩与解压
来源：http://zfi.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ire.hammf.cn

[R56] 远程拷贝
来源：http://qtn.nanxuanxn.top

scp file user@host:/path/
来源：http://ggf.xziqi.cn

[R57] 远程执行命令
来源：http://fap.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://ela.cucudq.cn

[R58] 下载文件
来源：http://pjw.ehwqpu.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wgz.dashuyun.cn

[R59] 发 POST JSON
来源：http://vxe.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bom.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://saz.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kuk.bjfxy.top

[R61] 磁盘占用
来源：http://sms.yfazqb.com

df -h;  du -sh *
来源：http://fzm.guannengcc.top

[R62] 找最占空间的文件
来源：http://utl.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://mgk.yanxiufei.cn

[R63] 内存与进程
来源：http://lor.birdmap.top

free -h;  ps aux | grep nginx
来源：http://vig.fktsv.cn

[R64] 结束进程
来源：http://cqs.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://xue.ydjk.org.cn

[R65] 查看端口占用
来源：http://rbv.ydjk.org.cn


<!-- 参考信息 -->