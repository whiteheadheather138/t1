代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://jvs.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bng.sufxvd.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fgm.hnxiangtu.top

[Q15] 查询全部
来源：http://fnj.jyoumei.cn

SELECT * FROM users;
来源：http://kdr.zdqjudy.top

[Q16] 查询指定列
来源：http://kyw.0kj1m.cn

SELECT id, name FROM users;
来源：http://muq.zdbjq.cn

[Q17] 条件查询
来源：http://wcb.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ueh.tanke756.top

[Q18] 模糊匹配
来源：http://uko.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eaj.dashuyun.cn

[Q19] 范围查询
来源：http://dcf.nanxinkj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fcy.guannengcc.top

[Q20] IN 列表
来源：http://etd.cdnleiting.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://alj.zdqjudy.top

[Q21] 空值判断
来源：http://gnv.zhaomingkeji.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://tsv.snrcjt.cn

[Q22] 排序
来源：http://eco.gzhubu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ztx.uphjek.com

[Q23] 分页
来源：http://ohy.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mvq.ctjpmb.com

[Q24] 去重
来源：http://cwy.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://jea.yonumen.top

[Q25] 只取前 N 条
来源：http://ian.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gpz.tian-w.cn

[Q26] 计数
来源：http://hyp.zhengqikj.top

SELECT COUNT(*) FROM users;
来源：http://dzz.yuxming.cn

[Q27] 条件计数
来源：http://qod.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://acr.xziqi.cn

[Q28] 求和与平均
来源：http://ntx.ydjk.org.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bmp.hywenlv.cn

[Q29] 最大最小值
来源：http://kxl.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zfn.jianghu66.top

[Q30] 分组统计
来源：http://tjy.snrcjt.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fxo.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://ktm.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://coe.andypj.xyz

[Q32] 分组拼接字符串
来源：http://lgt.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hkz.sweek.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sle.kuanghao11.cn

[Q33] 多列分组
来源：http://beo.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sim.ppjwa.cn

[Q34] 每组取第一条
来源：http://dnv.chenzaomai.com

SELECT * FROM (
来源：http://dri.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nwq.jqgfzy.top

) t WHERE rn = 1;
来源：http://sdo.fktsv.cn

[Q35] 内连接
来源：http://qgj.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gvh.zhixingplan.top

[Q36] 左连接
来源：http://xch.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://omm.yanxiufei.cn

[Q37] 右连接
来源：http://iwx.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zgv.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ohl.shanyushiyangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rly.chenzaomai.com

[Q39] 自连接（查上下级）
来源：http://qfk.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uju.tanke756.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://txa.jqgufenzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://icn.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lzz.ivvv.top

[Q41] 多表连接
来源：http://qjo.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://amr.havefunace.top

JOIN users u ON u.id = o.user_id
来源：http://rse.shanyushiyangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://ssh.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://xsu.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://bie.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xcr.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://ynh.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fdt.fehbvm.com

[Q44] IN 子查询
来源：http://sfl.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hce.yongpay.top

[Q45] EXISTS 判断存在
来源：http://dxa.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cjs.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pqk.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://swy.cqqwz.cn

[Q47] 与平均值比较
来源：http://yem.yongpay.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://smd.quarkkingdee.top

[Q48] CTE 公用表表达式
来源：http://hyn.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bqx.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://fcb.hnqzz.top

[Q49] 更新单行
来源：http://roa.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://otx.yanxiufei.cn

[Q50] 批量更新
来源：http://ciz.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://grc.zhijiandao.cn

[Q51] 用子查询更新
来源：http://oke.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pgb.hnqzz.top

[Q52] 删除指定行
来源：http://rqo.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://cbd.ybcxt.top

[Q53] 按条件删除
来源：http://pja.cucudq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://txg.yuxming.cn

[Q54] 清空表
来源：http://zyk.yj202588.top

TRUNCATE TABLE logs;
来源：http://bmp.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://xqa.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ehy.ydjk.org.cn

[Q56] 密集排名（并列不占位）
来源：http://myr.bjfxy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yvp.xuanzx.com

[Q57] 行号
来源：http://bni.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xxi.nanxinkj.top

[Q58] 累计求和
来源：http://ggo.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zzx.iojbl.cn

[Q59] 分组内累计
来源：http://zgp.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://prv.iojbl.cn

[Q60] 取上一行 / 下一行
来源：http://xsr.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ahh.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hgf.zycfv.cn

[Q61] 移动平均
来源：http://luz.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nry.vqdsnc.cn

[Q62] 分组占比
来源：http://zbq.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xym.quarkkingdee.top

[Q63] 开启事务
来源：http://svr.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://viz.kuanghao11.cn

[Q64] 提交事务
来源：http://pkl.chenlongwang.top

COMMIT;
来源：http://eyn.pycfn.com

[Q65] 回滚事务
来源：http://gze.vqdsnc.cn

ROLLBACK;
来源：http://nmg.hnxiangtu.top

[Q66] 行锁查询
来源：http://wci.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ted.zdbjq.cn

[Q67] 设置隔离级别
来源：http://gtx.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kuz.yj202588.top

[Q68] 保存点
来源：http://ile.hcnkem.com

SAVEPOINT sp1;
来源：http://rcq.c1oappe.top

ROLLBACK TO sp1;
来源：http://ysd.zhengqikj.top

[Q69] 查看执行计划
来源：http://hoi.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dxw.jianghu66.top

[Q70] 更新统计信息
来源：http://plq.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://hej.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://fyf.yuanzhike.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tco.zhixingplan.top

[Q72] 查看索引
来源：http://pgl.nanxuanxn.top

SHOW INDEX FROM users;
来源：http://njc.chenzaomai.com

[Q73] 查看表状态
来源：http://yix.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://iyi.pycfn.com

[Q74] 强制使用索引
来源：http://nud.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bna.shzxlz.cn

[Q75] 日期格式化
来源：http://vzs.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yvz.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mal.316326.xyz

[Q76] 按天统计
来源：http://fsv.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wwq.kuanghao11.cn

[Q77] 时间加减
来源：http://tsz.mhx1999.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vde.iojbl.cn

[Q78] 当前时间
来源：http://aaa.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wce.ppjwa.cn

[Q79] 字符串拼接
来源：http://gdl.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://alp.xuetiantiany.cn

[Q80] 字符串截取
来源：http://fka.zhongyouzk.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sdx.meibo888.top

[Q81] 字符串替换
来源：http://use.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ssb.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://rio.iojbl.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tsg.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://whs.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xrk.jinqigufen.top

[Q84] 去除首尾空格
来源：http://kzu.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://yiw.cqqwz.cn

[Q85] 数值取整
来源：http://jau.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://muc.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://ruy.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zyz.hongshengwenyu.top

[Q87] JSON 字段做条件
来源：http://xxr.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oxs.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://jog.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://prk.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sqk.andypj.xyz

[Q89] 判断表是否存在
来源：http://wxf.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://acd.nwbrower.top

[Q90] 生成序号列
来源：http://uno.daxiang520.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iro.jinyuanbaomall.cn

================================================================================
来源：http://iwl.wangdashe.top

R. Bash 专题
来源：http://kja.zhixingplan.top

================================================================================
来源：http://ymo.andypj.xyz

[R01] shebang 与严格模式
来源：http://ogg.c1oappe.top

#!/usr/bin/env bash
来源：http://vto.jinqigufen.top

set -euo pipefail
来源：http://axz.hnqzz.top

[R02] 变量赋值与使用
来源：http://ljl.birdmap.top

name="Tom"; echo "$name"
来源：http://vrb.zhiwuduotai.top

[R03] 只读变量
来源：http://pzz.uphjek.com

readonly PI=3.14
来源：http://hhn.tanke756.top

[R04] 位置参数
来源：http://qij.aizwys.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fln.daxiang520.top

[R05] 参数默认值
来源：http://ksw.hfpthk.cn

name="${1:-default}"
来源：http://fkb.cqqwz.cn

[R06] 判断命令是否存在
来源：http://ssf.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aex.dashuyun.cn

[R07] if 判断文件
来源：http://ydz.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ozc.shanyushiyangtech.top

[R08] 数值比较
来源：http://ztr.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://uga.hongshengwenyu.top

[R09] 字符串比较
来源：http://fdg.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zby.cheryme.top

[R10] 正则匹配
来源：http://szh.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://alc.yueranfly.top

[R11] case 多分支
来源：http://osx.xylfe.cn

case "$1" in
来源：http://nwr.tianlin.xyz

start) echo "启动" ;;
来源：http://rsj.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://ozr.iojbl.cn

*)     echo "未知命令" ;;
来源：http://bss.aibaodan.cn

esac
来源：http://mwt.cdnleiting.top

[R12] for 遍历文件
来源：http://xdv.fehbvm.com

for f in *.txt; do echo "$f"; done
来源：http://obk.fzhhl.top

[R13] for 计数循环
来源：http://wrf.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://wee.cdnleiting.top

[R14] C 风格 for
来源：http://sxq.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jqo.hnxiangtu.top

[R15] while 逐行读文件
来源：http://uua.hnxiangtu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://enp.tianlin.xyz

[R16] until 等待条件
来源：http://mne.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://meb.dashuyun.cn

[R17] 数组定义与取值
来源：http://den.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cvm.vqdsnc.cn

[R18] 遍历数组
来源：http://sco.yfazqb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://snb.yongpay.top

[R19] 数组长度
来源：http://muv.bbcook.cn

echo "${#arr[@]}"
来源：http://pvq.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://txa.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fkr.shzxlz.cn

[R21] 字符串长度
来源：http://jyk.jlsjyb.cn

echo "${#s}"
来源：http://xih.zhiwuduotai.top

[R22] 截取子串
来源：http://fwb.jiagoushi.top

echo "${s:0:5}"
来源：http://aia.vqdsnc.cn

[R23] 字符串替换
来源：http://pad.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ciy.andypj.xyz

[R24] 大小写转换
来源：http://ovr.sufxvd.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jwr.hnxiangtu.top

[R25] 去后缀 / 去前缀
来源：http://rbt.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ohx.52xcode.cn

[R26] 命令替换
来源：http://ckk.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://aps.hongshengwenyu.top

[R27] 算术展开
来源：http://qrn.yj202588.top

echo $((1 + 2 * 3))
来源：http://zzd.cdnleiting.top

[R28] 浮点运算
来源：http://nmw.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://buz.jiagoushi.top

[R29] 定义函数
来源：http://eow.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bvw.yj20258888.top

[R30] 函数返回状态码
来源：http://jfd.hongshengwenyu.top

f() { return 0; }; f || echo "失败了"
来源：http://hng.jlsjyb.cn

[R31] 局部变量
来源：http://ubn.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://oya.gzhubu.top

[R32] 参数个数校验
来源：http://qgq.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dop.shuidangran.top

[R33] 捕获错误并提示行号
来源：http://cdz.yj20258888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lsn.xuanzx.com

[R34] 退出时清理
来源：http://lqv.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kpa.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://ets.wangdashe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fgn.dianchejie.cn

[R36] 并发执行多个任务
来源：http://thg.hywenlv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zsn.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://lvr.iojbl.cn

files=$(ls -1)
来源：http://epy.jiagoushi.top

[R38] 管道串联
来源：http://lsx.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://uzq.sweek.top

[R39] 重定向标准输出与错误
来源：http://npp.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://dha.feifeiyinyue.top

[R40] 追加写日志
来源：http://jzc.shanyushiyangtech.top

echo "log" >> out.log
来源：http://rjn.yueranfly.top

[R41] 丢弃输出
来源：http://fce.jianghu66.top

cmd >/dev/null 2>&1
来源：http://ibd.gzhubu.top

[R42] 输入重定向
来源：http://wry.jyoumei.cn

wc -l < a.txt
来源：http://kpv.fehbvm.com

[R43] 按名字查找文件
来源：http://lzf.9152youxi.cn

find . -name "*.log" -type f
来源：http://ddu.c1oappe.top

[R44] 按修改时间查找
来源：http://aeg.yongpay.top

find . -mtime -7 -type f
来源：http://wgi.chenjidiqi.icu

[R45] 批量删除
来源：http://fpx.sweek.top

find . -name "*.tmp" -delete
来源：http://oqc.gaohongyu789.top

[R46] 递归替换文件内容
来源：http://vbq.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://crk.tanke756.top

[R47] sed 单行替换
来源：http://aqt.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://cid.jyoumei.cn

[R48] awk 取指定列
来源：http://kab.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://ztq.dashuyun.cn

[R49] awk 带条件
来源：http://omy.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yhp.birdmap.top

[R50] awk 求和
来源：http://vyi.fktsv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zth.svipenyu.cn

[R51] 排序去重取前几
来源：http://lhm.smart0.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ygx.hywenlv.cn

[R52] 统计行数
来源：http://uvt.yuxming.cn

wc -l a.txt
来源：http://nmh.jlsjyb.cn

[R53] 查看文件头与实时尾
来源：http://mce.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vgh.ppjwa.cn

[R54] 比较两个文件
来源：http://kgw.ctjpmb.com

diff a.txt b.txt
来源：http://mlg.zhongyouzk.top

[R55] 压缩与解压
来源：http://pyp.c1oappe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cxe.jinyuanbaomall.cn

[R56] 远程拷贝
来源：http://fnt.ppjwa.cn

scp file user@host:/path/
来源：http://ltd.hnqzz.top

[R57] 远程执行命令
来源：http://hlk.ehwqpu.com

ssh user@host 'uptime'
来源：http://reo.cheryme.top

[R58] 下载文件
来源：http://vke.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://diu.yonumen.top

[R59] 发 POST JSON
来源：http://wsk.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xgv.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://chs.yuanzhike.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://evf.zhiwuduotai.top

[R61] 磁盘占用
来源：http://uvn.daxiang520.top

df -h;  du -sh *
来源：http://pjh.chenlongwang.top

[R62] 找最占空间的文件
来源：http://smi.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://vcj.epnwcf.com

[R63] 内存与进程
来源：http://rex.0kj1m.cn


<!-- 参考信息 -->