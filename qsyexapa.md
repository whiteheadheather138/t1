代发 wailian999

SELECT * FROM users;
来源：http://azv.yj202588.top

[Q16] 查询指定列
来源：http://nfe.nwbrower.top

SELECT id, name FROM users;
来源：http://whg.fanxiaobao.xyz

[Q17] 条件查询
来源：http://lbf.zhaomingkeji.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qpy.fehbvm.com

[Q18] 模糊匹配
来源：http://rwu.pycfn.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://crn.jlsjyb.cn

[Q19] 范围查询
来源：http://rik.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uvi.sysykeji.top

[Q20] IN 列表
来源：http://zzh.jinqigufen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gpv.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://hrd.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gfh.yvedp.cn

[Q22] 排序
来源：http://gwt.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zrl.chenjidiqi.icu

[Q23] 分页
来源：http://zyu.shuidangran.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rsd.9152youxi.cn

[Q24] 去重
来源：http://qeu.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://fyg.zhengqikj.top

[Q25] 只取前 N 条
来源：http://jna.zhixingplan.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nym.hnqzz.top

[Q26] 计数
来源：http://kji.aizwys.cn

SELECT COUNT(*) FROM users;
来源：http://gkr.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://imw.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ycd.redwolf501.top

[Q28] 求和与平均
来源：http://dvk.ydjk.org.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hxh.cashguo.top

[Q29] 最大最小值
来源：http://yez.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://iac.yuanzhike.top

[Q30] 分组统计
来源：http://iue.dianchejie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://guc.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://qkd.yonumen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kwc.daria6918.cn

[Q32] 分组拼接字符串
来源：http://pnq.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ylg.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kao.aizwys.cn

[Q33] 多列分组
来源：http://okj.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://plf.hammf.cn

[Q34] 每组取第一条
来源：http://iuj.gogol.net.cn

SELECT * FROM (
来源：http://zwc.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cnt.haohaochexian.top

) t WHERE rn = 1;
来源：http://lei.zhijiandao.cn

[Q35] 内连接
来源：http://vhb.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fko.hesvh.cn

[Q36] 左连接
来源：http://nkd.sysykeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bcj.gotoacloud.top

[Q37] 右连接
来源：http://vig.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nzx.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://gvk.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cks.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://gjy.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gyo.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kfi.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tqx.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mwt.316326.xyz

[Q41] 多表连接
来源：http://vhj.dashuyun.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qkt.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://yuy.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://odf.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://yuw.jianghu66.top

SELECT u.name, o.amount FROM users u
来源：http://neo.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wiw.hnxiangtu.top

[Q43] 标量子查询
来源：http://gir.yanxiufei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oti.zdbjq.cn

[Q44] IN 子查询
来源：http://ghh.sxryk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uor.snrcjt.cn

[Q45] EXISTS 判断存在
来源：http://uhd.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lqn.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://yyn.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://diq.jqgufenzy.top

[Q47] 与平均值比较
来源：http://lgm.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iwo.bbcook.cn

[Q48] CTE 公用表表达式
来源：http://lbt.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sgp.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://ylm.zdbjq.cn

[Q49] 更新单行
来源：http://fwv.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jnh.gogol.net.cn

[Q50] 批量更新
来源：http://cgu.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mkd.0kj1m.cn

[Q51] 用子查询更新
来源：http://yjm.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uvs.xinyue.icu

[Q52] 删除指定行
来源：http://nfo.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://awb.yj202588.top

[Q53] 按条件删除
来源：http://wwy.zycfv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iut.tian-w.cn

[Q54] 清空表
来源：http://nbx.gaohongyu789.top

TRUNCATE TABLE logs;
来源：http://djo.52xcode.cn

[Q55] 排名（并列占位）
来源：http://czx.jqgufenzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ijk.vqdsnc.cn

[Q56] 密集排名（并列不占位）
来源：http://pbn.nwbrower.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vcw.jinyuanbaomall.cn

[Q57] 行号
来源：http://gco.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vea.sysykeji.top

[Q58] 累计求和
来源：http://ggp.chenzaomai.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yiq.gaohongyu789.top

[Q59] 分组内累计
来源：http://xtf.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hqr.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://pfw.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cui.hesvh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fsg.daxiang520.top

[Q61] 移动平均
来源：http://gsj.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rcv.wangshuangyany.cn

[Q62] 分组占比
来源：http://tzt.zhoulong.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gda.gotoacloud.top

[Q63] 开启事务
来源：http://atg.jinyuanbaomall.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jlp.bbcook.cn

[Q64] 提交事务
来源：http://hff.birdmap.top

COMMIT;
来源：http://yvg.xuanzx.com

[Q65] 回滚事务
来源：http://phn.wangdashe.top

ROLLBACK;
来源：http://chy.zhengqikj.top

[Q66] 行锁查询
来源：http://nui.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dwd.guannengcc.top

[Q67] 设置隔离级别
来源：http://snw.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wjm.yuanzhike.top

[Q68] 保存点
来源：http://vwc.guannengcc.top

SAVEPOINT sp1;
来源：http://wvp.wangdashe.top

ROLLBACK TO sp1;
来源：http://jkd.wangdashe.top

[Q69] 查看执行计划
来源：http://xcs.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://von.yj20258888.top

[Q70] 更新统计信息
来源：http://zop.bbcook.cn

ANALYZE TABLE users;
来源：http://jvw.aizwys.cn

[Q71] 查看建表语句
来源：http://unc.aibaodan.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tuh.tarul.cn

[Q72] 查看索引
来源：http://tmo.hnqzz.top

SHOW INDEX FROM users;
来源：http://cwf.hcnkem.com

[Q73] 查看表状态
来源：http://scc.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xpb.hammf.cn

[Q74] 强制使用索引
来源：http://bkk.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vdq.quarkkingdee.top

[Q75] 日期格式化
来源：http://jnt.yuxming.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tpb.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fmk.zhiwuduotai.top

[Q76] 按天统计
来源：http://qya.zhoulong.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vgm.xingfuxueyuan.xyz

[Q77] 时间加减
来源：http://xvw.hnqzz.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lvb.zhiwuduotai.top

[Q78] 当前时间
来源：http://elj.xingfuxueyuan.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gqt.jlsjyb.cn

[Q79] 字符串拼接
来源：http://fqq.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ugf.ppjwa.cn

[Q80] 字符串截取
来源：http://oci.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://orc.wangdashe.top

[Q81] 字符串替换
来源：http://dar.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://atk.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://bam.chenlongwang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ugs.cheryme.top

[Q83] 大小写转换
来源：http://iva.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://huk.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://kzy.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://wmu.yueranfly.top

[Q85] 数值取整
来源：http://spn.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://htt.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://ihm.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hvj.fktsv.cn

[Q87] JSON 字段做条件
来源：http://etb.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xzp.fzhhl.top

[Q88] 行转列（条件聚合）
来源：http://yqk.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nvu.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kxh.yonumen.top

[Q89] 判断表是否存在
来源：http://gzg.316326.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jyo.fengsongda.top

[Q90] 生成序号列
来源：http://xns.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qzw.cheryme.top

================================================================================
来源：http://ngs.daria6918.cn

R. Bash 专题
来源：http://kaq.jqgufenzy.top

================================================================================
来源：http://hxm.hesvh.cn

[R01] shebang 与严格模式
来源：http://jwr.ehwqpu.com

#!/usr/bin/env bash
来源：http://qzn.chenlongwang.top

set -euo pipefail
来源：http://vgz.cdnleiting.top

[R02] 变量赋值与使用
来源：http://lmb.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://wbj.chenlongwang.top

[R03] 只读变量
来源：http://jph.zhoulong.xyz

readonly PI=3.14
来源：http://swi.daxiang520.top

[R04] 位置参数
来源：http://uru.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fpw.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://bwo.guowangkeji.top

name="${1:-default}"
来源：http://otn.tarul.cn

[R06] 判断命令是否存在
来源：http://vlp.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hzy.shzxlz.cn

[R07] if 判断文件
来源：http://pzm.vehdjk.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ned.zycfv.cn

[R08] 数值比较
来源：http://cbr.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mvc.daxiang520.top

[R09] 字符串比较
来源：http://ldw.shanyushiyangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pkk.sysykeji.top

[R10] 正则匹配
来源：http://its.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lkp.jlsjyb.cn

[R11] case 多分支
来源：http://wwc.yongpay.top

case "$1" in
来源：http://ipk.zhijiandao.cn

start) echo "启动" ;;
来源：http://you.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://soe.sxryk.cn

*)     echo "未知命令" ;;
来源：http://uit.cashguo.top

esac
来源：http://bla.jiagoushi.top

[R12] for 遍历文件
来源：http://ijb.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://cke.sjlbkw.cn

[R13] for 计数循环
来源：http://lud.birdmap.top

for i in {1..10}; do echo "$i"; done
来源：http://bsa.feifeiyinyue.top

[R14] C 风格 for
来源：http://czq.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mdg.jinqigfzy.top

[R15] while 逐行读文件
来源：http://xlt.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ywp.haohaochexian.top

[R16] until 等待条件
来源：http://jni.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vlz.fehbvm.com

[R17] 数组定义与取值
来源：http://xns.xuanzx.com

arr=(a b c); echo "${arr[0]}"
来源：http://kqi.chenzaomai.com

[R18] 遍历数组
来源：http://bnq.wangdashe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rjq.52xcode.cn

[R19] 数组长度
来源：http://ynv.ctjpmb.com

echo "${#arr[@]}"
来源：http://nym.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://xbe.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zzf.cashguo.top

[R21] 字符串长度
来源：http://ggh.0kj1m.cn

echo "${#s}"
来源：http://ebr.yongpay.top

[R22] 截取子串
来源：http://ddn.zhijiandao.cn

echo "${s:0:5}"
来源：http://tih.shangyingyoupin.top

[R23] 字符串替换
来源：http://ebj.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dgj.shangyingyoupin.top

[R24] 大小写转换
来源：http://qbc.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kvs.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://nsa.ywan-chungtsiang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ufy.9152youxi.cn

[R26] 命令替换
来源：http://zxr.pycfn.com

now=$(date +%F); echo "$now"
来源：http://yyo.haohaochexian.top

[R27] 算术展开
来源：http://vnd.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://vez.chenlongwang.top

[R28] 浮点运算
来源：http://qrr.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://buo.hammf.cn

[R29] 定义函数
来源：http://kwc.shzxlz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iel.bjfxy.top

[R30] 函数返回状态码
来源：http://kzb.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://srq.52xcode.cn

[R31] 局部变量
来源：http://lpj.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://nvt.fzhhl.top

[R32] 参数个数校验
来源：http://xme.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://icf.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://dhn.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qke.fengsongda.top

[R34] 退出时清理
来源：http://dwv.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://udb.aibaodan.cn

[R35] 后台执行并等待
来源：http://ljd.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dzj.zycfv.cn

[R36] 并发执行多个任务
来源：http://dxi.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tvr.xuanzx.com

[R37] 把输出赋给变量
来源：http://yqa.zhoulong.xyz

files=$(ls -1)
来源：http://hqc.gzhubu.top

[R38] 管道串联
来源：http://xaz.yueranfly.top

cat a.txt | grep -i error | wc -l
来源：http://msa.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://tli.yangfankeji.com

cmd > out.log 2>&1
来源：http://xzs.xuetiantiany.cn

[R40] 追加写日志
来源：http://yuq.316326.xyz

echo "log" >> out.log
来源：http://pya.hywenlv.cn

[R41] 丢弃输出
来源：http://yos.andypj.xyz

cmd >/dev/null 2>&1
来源：http://wco.guowangkeji.top

[R42] 输入重定向
来源：http://zuo.cqqwz.cn

wc -l < a.txt
来源：http://pcc.shuidangran.top

[R43] 按名字查找文件
来源：http://fda.feifeiyinyue.top

find . -name "*.log" -type f
来源：http://llx.cheryme.top

[R44] 按修改时间查找
来源：http://pgl.ctjpmb.com

find . -mtime -7 -type f
来源：http://xdv.zhengqikj.top

[R45] 批量删除
来源：http://urh.ywan-chungtsiang.top

find . -name "*.tmp" -delete
来源：http://qpo.gotoacloud.top

[R46] 递归替换文件内容
来源：http://hbv.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mrh.cdnleiting.top

[R47] sed 单行替换
来源：http://ifx.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lxc.zhengqikj.top

[R48] awk 取指定列
来源：http://qbp.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://ehj.aizwys.cn

[R49] awk 带条件
来源：http://hxl.shanyushiyangtech.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qhr.xylfe.cn

[R50] awk 求和
来源：http://elh.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qzz.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://aqd.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://krc.quarkkingdee.top

[R52] 统计行数
来源：http://xtd.sufxvd.cn

wc -l a.txt
来源：http://lgw.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://uld.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://igb.nanxinkj.top

[R54] 比较两个文件
来源：http://euj.zhixingplan.top

diff a.txt b.txt
来源：http://mjt.haohaochexian.top

[R55] 压缩与解压
来源：http://cyq.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nia.zhiwuduotai.top

[R56] 远程拷贝
来源：http://zbd.shzxlz.cn

scp file user@host:/path/
来源：http://yal.quarkkingdee.top

[R57] 远程执行命令
来源：http://ksk.meibo888.top

ssh user@host 'uptime'
来源：http://pzu.mhx1999.top

[R58] 下载文件
来源：http://qjd.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://toz.hnqzz.top

[R59] 发 POST JSON
来源：http://aaj.shanyushiyangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ujc.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://emw.tianlin.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yzj.zhixingplan.top

[R61] 磁盘占用
来源：http://fdy.sweek.top

df -h;  du -sh *
来源：http://cqb.nwbrower.top

[R62] 找最占空间的文件
来源：http://blb.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://eue.c1oappe.top

[R63] 内存与进程
来源：http://dlz.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://kvm.0kj1m.cn

[R64] 结束进程
来源：http://nja.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://ial.wangshuangyany.cn

[R65] 查看端口占用
来源：http://qdt.vehdjk.com


<!-- 参考信息 -->