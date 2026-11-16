代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://qdm.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tgh.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pyq.dianchejie.cn

[Q15] 查询全部
来源：http://wxe.yvedp.cn

SELECT * FROM users;
来源：http://wbw.fehbvm.com

[Q16] 查询指定列
来源：http://hrx.hammf.cn

SELECT id, name FROM users;
来源：http://itx.birdmap.top

[Q17] 条件查询
来源：http://sjv.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hsr.zycfv.cn

[Q18] 模糊匹配
来源：http://zup.sweek.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://roq.snrcjt.cn

[Q19] 范围查询
来源：http://mbn.jinyuanbaomall.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qoi.mhx1999.top

[Q20] IN 列表
来源：http://mhe.nanxinkj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rci.jlsjyb.cn

[Q21] 空值判断
来源：http://coj.ivvv.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gvd.yj20258888.top

[Q22] 排序
来源：http://qrm.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://twa.yj20258888.top

[Q23] 分页
来源：http://ttz.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mon.zhoulong.xyz

[Q24] 去重
来源：http://ixe.haohaochexian.top

SELECT DISTINCT city FROM users;
来源：http://qka.xingfuxueyuan.xyz

[Q25] 只取前 N 条
来源：http://tok.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wbo.zdqjudy.top

[Q26] 计数
来源：http://wcs.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://ntd.c1oappe.top

[Q27] 条件计数
来源：http://ppo.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rqw.zdqjudy.top

[Q28] 求和与平均
来源：http://gmn.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yxm.wangdashe.top

[Q29] 最大最小值
来源：http://myv.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jhs.yfazqb.com

[Q30] 分组统计
来源：http://ant.sxryk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dyi.shzxlz.cn

[Q31] 分组后过滤
来源：http://ocu.chenjidiqi.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://smp.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://gde.kuanghao11.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vaj.fktsv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ogz.aibaodan.cn

[Q33] 多列分组
来源：http://ogw.pycfn.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wbg.daria6918.cn

[Q34] 每组取第一条
来源：http://ubh.cheryme.top

SELECT * FROM (
来源：http://uku.9152youxi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uti.bjfxy.top

) t WHERE rn = 1;
来源：http://ahk.ydjk.org.cn

[Q35] 内连接
来源：http://nvr.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gzr.shanyushiyangkeji.top

[Q36] 左连接
来源：http://ykr.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tqf.jianghu66.top

[Q37] 右连接
来源：http://nlx.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yzi.pengpengdd.cyou

[Q38] 全外连接（PostgreSQL）
来源：http://hxd.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oqa.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://hpv.guowangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hqq.xuetiantiany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fuv.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://wxs.fzhhl.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dva.hnxiangtu.top

[Q41] 多表连接
来源：http://lgi.hesvh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://njm.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://jok.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://jcf.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://ztq.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://umt.fanxiaobao.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nzr.jinghuilouyu.cn

[Q43] 标量子查询
来源：http://gbi.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qzn.hcnkem.com

[Q44] IN 子查询
来源：http://xhw.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lws.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://rke.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aap.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://ocs.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zec.nanxuanxn.top

[Q47] 与平均值比较
来源：http://sts.mhx1999.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://quj.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://uft.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bpz.hammf.cn

SELECT * FROM t WHERE c > 5;
来源：http://dmo.yuanzhike.top

[Q49] 更新单行
来源：http://euf.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cja.xuetiantiany.cn

[Q50] 批量更新
来源：http://wbg.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ztq.zdbjq.cn

[Q51] 用子查询更新
来源：http://ppq.guannengcc.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eky.fanxiaobao.xyz

[Q52] 删除指定行
来源：http://twc.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://mzy.jlsjyb.cn

[Q53] 按条件删除
来源：http://otw.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ljd.hcnkem.com

[Q54] 清空表
来源：http://maj.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://xwt.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://qur.daxiang520.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tmn.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://cwr.hammf.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ueq.jyoumei.cn

[Q57] 行号
来源：http://ome.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jws.tanke756.top

[Q58] 累计求和
来源：http://aov.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xvd.nwbrower.top

[Q59] 分组内累计
来源：http://gbh.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://plq.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://sky.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iqk.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iks.52xcode.cn

[Q61] 移动平均
来源：http://mul.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ipj.quarkkingdee.top

[Q62] 分组占比
来源：http://lmu.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pms.gogol.net.cn

[Q63] 开启事务
来源：http://pmq.fehbvm.com

START TRANSACTION;                -- 或 BEGIN
来源：http://gnn.xziqi.cn

[Q64] 提交事务
来源：http://vio.cdnleiting.top

COMMIT;
来源：http://wkz.gotoacloud.top

[Q65] 回滚事务
来源：http://gfc.zdqjudy.top

ROLLBACK;
来源：http://skp.zhijiandao.cn

[Q66] 行锁查询
来源：http://tdc.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ghf.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://lhg.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xqb.hammf.cn

[Q68] 保存点
来源：http://sfj.shzxlz.cn

SAVEPOINT sp1;
来源：http://bfo.epnwcf.com

ROLLBACK TO sp1;
来源：http://byg.9152youxi.cn

[Q69] 查看执行计划
来源：http://kfo.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oqg.meibo888.top

[Q70] 更新统计信息
来源：http://sea.0kj1m.cn

ANALYZE TABLE users;
来源：http://opf.cheryme.top

[Q71] 查看建表语句
来源：http://nfj.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hut.kuanghao11.cn

[Q72] 查看索引
来源：http://hzq.sufxvd.cn

SHOW INDEX FROM users;
来源：http://trm.cashguo.top

[Q73] 查看表状态
来源：http://fms.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://erg.havefunace.top

[Q74] 强制使用索引
来源：http://gdm.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gky.daria6918.cn

[Q75] 日期格式化
来源：http://pbo.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://inu.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ver.zycfv.cn

[Q76] 按天统计
来源：http://uns.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wvm.redwolf501.top

[Q77] 时间加减
来源：http://ptw.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qze.shangyingyoupin.top

[Q78] 当前时间
来源：http://xfg.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lbl.aibaodan.cn

[Q79] 字符串拼接
来源：http://qnp.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rfo.nwbrower.top

[Q80] 字符串截取
来源：http://eno.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wup.sysykeji.top

[Q81] 字符串替换
来源：http://ntb.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mld.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://rhi.zycfv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zqy.yongpay.top

[Q83] 大小写转换
来源：http://lgt.cqqwz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://exc.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://ogn.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://wok.jianghu66.top

[Q85] 数值取整
来源：http://dpb.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gfr.hnxiangtu.top

[Q86] 读取 JSON 字段
来源：http://hfv.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://atw.fehbvm.com

[Q87] JSON 字段做条件
来源：http://ipv.jiagoushi.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wya.52xcode.cn

[Q88] 行转列（条件聚合）
来源：http://tqe.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ydz.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bsr.wangdashe.top

[Q89] 判断表是否存在
来源：http://mrr.shanyushiyangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kwv.yuxming.cn

[Q90] 生成序号列
来源：http://wqt.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bcd.bjfxy.top

================================================================================
来源：http://noj.gaohongyu789.top

R. Bash 专题
来源：http://yrk.jqgfzy.top

================================================================================
来源：http://kxv.dianchejie.cn

[R01] shebang 与严格模式
来源：http://xpe.hnqzz.top

#!/usr/bin/env bash
来源：http://dyw.ehwqpu.com

set -euo pipefail
来源：http://kew.zhijiandao.cn

[R02] 变量赋值与使用
来源：http://mhc.shzxlz.cn

name="Tom"; echo "$name"
来源：http://fae.jqgfzy.top

[R03] 只读变量
来源：http://wte.ehwqpu.com

readonly PI=3.14
来源：http://zgk.yueranfly.top

[R04] 位置参数
来源：http://piq.chenzaomai.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xfw.hywenlv.cn

[R05] 参数默认值
来源：http://gwj.316326.xyz

name="${1:-default}"
来源：http://ghm.hfpthk.cn

[R06] 判断命令是否存在
来源：http://sbu.jlsjyb.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pys.sxryk.cn

[R07] if 判断文件
来源：http://vpy.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tfs.gaohongyu789.top

[R08] 数值比较
来源：http://syk.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://phn.ydjk.org.cn

[R09] 字符串比较
来源：http://giu.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vqo.ctjpmb.com

[R10] 正则匹配
来源：http://shv.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gab.meibo888.top

[R11] case 多分支
来源：http://gtq.yj20258.top

case "$1" in
来源：http://qut.bbcook.cn

start) echo "启动" ;;
来源：http://ucv.tianlin.xyz

stop)  echo "停止" ;;
来源：http://pfj.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://iaa.jinqigufen.top

esac
来源：http://dnn.ivvv.top

[R12] for 遍历文件
来源：http://swp.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://wue.jinyuanbaomall.cn

[R13] for 计数循环
来源：http://wsb.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://pvc.daxiang520.top

[R14] C 风格 for
来源：http://kaj.zhiwuduotai.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lrp.cashguo.top

[R15] while 逐行读文件
来源：http://zdb.meibo888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lzl.hnxiangtu.top

[R16] until 等待条件
来源：http://gbi.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://snr.0kj1m.cn

[R17] 数组定义与取值
来源：http://peb.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qdr.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://djg.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hsh.shangyingyoupin.top

[R19] 数组长度
来源：http://zdy.gzhubu.top

echo "${#arr[@]}"
来源：http://rad.sysykeji.top

[R20] 关联数组（字典）
来源：http://gsi.fktsv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ujk.daria6918.cn

[R21] 字符串长度
来源：http://ugk.haohaochexian.top

echo "${#s}"
来源：http://hnh.ydzc1.top

[R22] 截取子串
来源：http://yne.wangshuangyany.cn

echo "${s:0:5}"
来源：http://ror.0kj1m.cn

[R23] 字符串替换
来源：http://org.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ags.hywenlv.cn

[R24] 大小写转换
来源：http://iam.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jjo.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://gwx.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dyw.iojbl.cn

[R26] 命令替换
来源：http://lar.nanxuanxn.top

now=$(date +%F); echo "$now"
来源：http://myu.zdqjudy.top

[R27] 算术展开
来源：http://ujf.yj20258888.top

echo $((1 + 2 * 3))
来源：http://iey.sjlbkw.cn

[R28] 浮点运算
来源：http://myv.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://jho.nanxinkj.top

[R29] 定义函数
来源：http://mpp.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eyp.sxryk.cn

[R30] 函数返回状态码
来源：http://mjy.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://qod.gaohongyu789.top

[R31] 局部变量
来源：http://wrt.gzhubu.top

f() { local x=1; echo "$x"; }
来源：http://adu.mhx1999.top

[R32] 参数个数校验
来源：http://wmr.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cih.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://rpz.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oyl.cdnleiting.top

[R34] 退出时清理
来源：http://lru.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://sah.yj20258.top

[R35] 后台执行并等待
来源：http://tgo.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://zrq.9152youxi.cn

[R36] 并发执行多个任务
来源：http://jex.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tmu.xziqi.cn

[R37] 把输出赋给变量
来源：http://hki.epnwcf.com

files=$(ls -1)
来源：http://ech.tianlin.xyz

[R38] 管道串联
来源：http://fml.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://zgr.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://qyo.jinqigufen.top

cmd > out.log 2>&1
来源：http://vau.yongpay.top

[R40] 追加写日志
来源：http://qvy.vqdsnc.cn

echo "log" >> out.log
来源：http://qow.cdnleiting.top

[R41] 丢弃输出
来源：http://uxy.shuidangran.top

cmd >/dev/null 2>&1
来源：http://xml.yueranfly.top

[R42] 输入重定向
来源：http://bvo.jinghuilouyu.cn

wc -l < a.txt
来源：http://kia.52xcode.cn

[R43] 按名字查找文件
来源：http://wvk.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://wsl.epnwcf.com

[R44] 按修改时间查找
来源：http://hya.sjlbkw.cn

find . -mtime -7 -type f
来源：http://scf.xuanzx.com

[R45] 批量删除
来源：http://hcb.ybcxt.top

find . -name "*.tmp" -delete
来源：http://krq.hnqzz.top

[R46] 递归替换文件内容
来源：http://nko.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wvw.cqqwz.cn

[R47] sed 单行替换
来源：http://hir.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bvg.xinyue.icu

[R48] awk 取指定列
来源：http://vhx.hammf.cn

awk '{print $1, $3}' a.txt
来源：http://ard.xinyue.icu

[R49] awk 带条件
来源：http://lod.zhiwuduotai.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://doy.epnwcf.com

[R50] awk 求和
来源：http://raj.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://ksg.bjfxy.top

[R51] 排序去重取前几
来源：http://okd.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://icu.sjlbkw.cn

[R52] 统计行数
来源：http://onv.mhx1999.top

wc -l a.txt
来源：http://rqe.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://oto.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nsg.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://lbo.nanxuanxn.top

diff a.txt b.txt
来源：http://rtd.daria6918.cn

[R55] 压缩与解压
来源：http://wip.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://raj.bjfxy.top

[R56] 远程拷贝
来源：http://xgr.dianchejie.cn

scp file user@host:/path/
来源：http://mxq.haohaochexian.top

[R57] 远程执行命令
来源：http://avl.zhoulong.xyz

ssh user@host 'uptime'
来源：http://hyy.pengpengdd.cyou

[R58] 下载文件
来源：http://wwy.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qmi.xylfe.cn

[R59] 发 POST JSON
来源：http://bfm.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pqs.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://ipr.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wwg.zdbjq.cn

[R61] 磁盘占用
来源：http://wfb.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://bqj.gzhubu.top

[R62] 找最占空间的文件
来源：http://osv.yonumen.top

du -ah . | sort -rh | head -10
来源：http://fmk.meibo888.top

[R63] 内存与进程
来源：http://nsd.hongshengwenyu.top


<!-- 参考信息 -->