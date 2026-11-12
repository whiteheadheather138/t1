代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://zvz.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dxd.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gxm.ivvv.top

[Q15] 查询全部
来源：http://bou.0kj1m.cn

SELECT * FROM users;
来源：http://xtt.zdqjudy.top

[Q16] 查询指定列
来源：http://frh.ehwqpu.com

SELECT id, name FROM users;
来源：http://idi.aizwys.cn

[Q17] 条件查询
来源：http://blf.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pao.xziqi.cn

[Q18] 模糊匹配
来源：http://cwg.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vqr.ydzc1.top

[Q19] 范围查询
来源：http://qvy.cqqwz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zza.shzxlz.cn

[Q20] IN 列表
来源：http://pix.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uwj.iojbl.cn

[Q21] 空值判断
来源：http://xux.redwolf501.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gdl.fktsv.cn

[Q22] 排序
来源：http://pao.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zcu.mhx1999.top

[Q23] 分页
来源：http://hbh.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pcx.hnxiangtu.top

[Q24] 去重
来源：http://kpl.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://rcf.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://gvl.wangshuangyany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://obh.pycfn.com

[Q26] 计数
来源：http://trf.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://qbt.jyoumei.cn

[Q27] 条件计数
来源：http://qkm.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ggr.zdbjq.cn

[Q28] 求和与平均
来源：http://ytm.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://arj.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://iko.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://moi.gaohongyu789.top

[Q30] 分组统计
来源：http://ixr.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tbg.xinyue.icu

[Q31] 分组后过滤
来源：http://bho.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cml.tian-w.cn

[Q32] 分组拼接字符串
来源：http://tly.hnxiangtu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ljz.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ylw.pengpengdd.cyou

[Q33] 多列分组
来源：http://kcy.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ssj.haohaochexian.top

[Q34] 每组取第一条
来源：http://trw.tarul.cn

SELECT * FROM (
来源：http://cru.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eui.daxiang520.top

) t WHERE rn = 1;
来源：http://aiu.cucudq.cn

[Q35] 内连接
来源：http://xgc.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hqh.shangyingyoupin.top

[Q36] 左连接
来源：http://rkx.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://czh.cucudq.cn

[Q37] 右连接
来源：http://jho.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pau.guannengcc.top

[Q38] 全外连接（PostgreSQL）
来源：http://fqx.jiagoushi.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sjh.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://czx.daxiang520.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ktj.ppjwa.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qkn.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ptn.aizwys.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dps.sufxvd.cn

[Q41] 多表连接
来源：http://hyz.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ogl.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://unb.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://dln.svipenyu.cn

[Q42] 连接条件附加过滤
来源：http://qny.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://gpy.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sbr.sweek.top

[Q43] 标量子查询
来源：http://mxj.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zlb.zhengqikj.top

[Q44] IN 子查询
来源：http://ssc.haohaochexian.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ahw.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://oys.yuanzhike.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://czx.svipenyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ajo.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kxt.quarkkingdee.top

[Q47] 与平均值比较
来源：http://ahy.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ljn.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://yzv.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hoc.zhengqikj.top

SELECT * FROM t WHERE c > 5;
来源：http://yyk.xylfe.cn

[Q49] 更新单行
来源：http://zva.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ibq.hnxiangtu.top

[Q50] 批量更新
来源：http://wpn.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nmh.xziqi.cn

[Q51] 用子查询更新
来源：http://zpz.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yst.52xcode.cn

[Q52] 删除指定行
来源：http://sgq.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://yxw.nwbrower.top

[Q53] 按条件删除
来源：http://bcp.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ncl.zdqjudy.top

[Q54] 清空表
来源：http://yie.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://eke.yongpay.top

[Q55] 排名（并列占位）
来源：http://wih.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ldy.fanxiaobao.xyz

[Q56] 密集排名（并列不占位）
来源：http://sgl.chenlongwang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hjw.nanxinkj.top

[Q57] 行号
来源：http://can.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xgo.fktsv.cn

[Q58] 累计求和
来源：http://yix.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ofp.pengpengdd.cyou

[Q59] 分组内累计
来源：http://nhw.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iqz.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://hpk.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jev.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zgj.cqqwz.cn

[Q61] 移动平均
来源：http://ddr.pycfn.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lex.cheryme.top

[Q62] 分组占比
来源：http://mmx.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://spn.fzhhl.top

[Q63] 开启事务
来源：http://ytn.ctjpmb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://unu.hnxiangtu.top

[Q64] 提交事务
来源：http://ibf.xylfe.cn

COMMIT;
来源：http://zfr.zycfv.cn

[Q65] 回滚事务
来源：http://fxz.cashguo.top

ROLLBACK;
来源：http://sar.chenjidiqi.icu

[Q66] 行锁查询
来源：http://cvg.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fkh.yj20258.top

[Q67] 设置隔离级别
来源：http://rxd.yuanzhike.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zsv.mhx1999.top

[Q68] 保存点
来源：http://xkz.cheryme.top

SAVEPOINT sp1;
来源：http://vsb.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://eqs.xingfuxueyuan.xyz

[Q69] 查看执行计划
来源：http://hav.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sdu.yonumen.top

[Q70] 更新统计信息
来源：http://hyx.0kj1m.cn

ANALYZE TABLE users;
来源：http://doa.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://uyx.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fcr.fehbvm.com

[Q72] 查看索引
来源：http://olh.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://orl.xinyue.icu

[Q73] 查看表状态
来源：http://cri.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://eyd.tarul.cn

[Q74] 强制使用索引
来源：http://wnd.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vlx.cashguo.top

[Q75] 日期格式化
来源：http://qqe.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fqq.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jiu.quarkkingdee.top

[Q76] 按天统计
来源：http://zag.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zhn.hesvh.cn

[Q77] 时间加减
来源：http://qhf.cdnleiting.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xet.yueranfly.top

[Q78] 当前时间
来源：http://ivy.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qiu.yj20258888.top

[Q79] 字符串拼接
来源：http://zhk.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hyp.sweek.top

[Q80] 字符串截取
来源：http://jaz.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wgo.wangshuangyany.cn

[Q81] 字符串替换
来源：http://wdt.shanyushiyangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kpe.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://qki.bbcook.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zfp.ehwqpu.com

[Q83] 大小写转换
来源：http://kxm.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nbs.cheryme.top

[Q84] 去除首尾空格
来源：http://cih.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://bwt.cdnleiting.top

[Q85] 数值取整
来源：http://xxd.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qiw.yuanzhike.top

[Q86] 读取 JSON 字段
来源：http://vzt.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nhz.yueranfly.top

[Q87] JSON 字段做条件
来源：http://hxd.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wox.fzhhl.top

[Q88] 行转列（条件聚合）
来源：http://zfw.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lfz.ywan-chungtsiang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pvo.ppjwa.cn

[Q89] 判断表是否存在
来源：http://dph.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sob.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://qfc.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nwc.gogol.net.cn

================================================================================
来源：http://gib.jinqigufen.top

R. Bash 专题
来源：http://ryy.hcnkem.com

================================================================================
来源：http://xop.pycfn.com

[R01] shebang 与严格模式
来源：http://kct.nanxuanxn.top

#!/usr/bin/env bash
来源：http://pkd.zdbjq.cn

set -euo pipefail
来源：http://kym.yangfankeji.com

[R02] 变量赋值与使用
来源：http://lmz.aibaodan.cn

name="Tom"; echo "$name"
来源：http://ikf.mhx1999.top

[R03] 只读变量
来源：http://qui.jqgufenzy.top

readonly PI=3.14
来源：http://rlk.shanyushiyangtech.top

[R04] 位置参数
来源：http://nph.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ebf.yfazqb.com

[R05] 参数默认值
来源：http://upd.0kj1m.cn

name="${1:-default}"
来源：http://loo.cqqwz.cn

[R06] 判断命令是否存在
来源：http://wql.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jdh.meibo888.top

[R07] if 判断文件
来源：http://avd.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gei.jqgfzy.top

[R08] 数值比较
来源：http://eed.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zqe.haohaochexian.top

[R09] 字符串比较
来源：http://uyh.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bks.chenzaomai.com

[R10] 正则匹配
来源：http://qtb.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://syy.zhaomingkeji.xyz

[R11] case 多分支
来源：http://yyd.gogol.net.cn

case "$1" in
来源：http://jdi.snrcjt.cn

start) echo "启动" ;;
来源：http://cgt.ppjwa.cn

stop)  echo "停止" ;;
来源：http://rfp.xinyue.icu

*)     echo "未知命令" ;;
来源：http://zgv.sjlbkw.cn

esac
来源：http://nfv.fktsv.cn

[R12] for 遍历文件
来源：http://jfq.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://yvz.aibaodan.cn

[R13] for 计数循环
来源：http://yia.xylfe.cn

for i in {1..10}; do echo "$i"; done
来源：http://uuq.0kj1m.cn

[R14] C 风格 for
来源：http://lxr.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oim.0kj1m.cn

[R15] while 逐行读文件
来源：http://lfu.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aop.tanke756.top

[R16] until 等待条件
来源：http://hze.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wkr.tianlin.xyz

[R17] 数组定义与取值
来源：http://yii.aibaodan.cn

arr=(a b c); echo "${arr[0]}"
来源：http://omf.xylfe.cn

[R18] 遍历数组
来源：http://miu.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ryb.andypj.xyz

[R19] 数组长度
来源：http://rwo.yj20258.top

echo "${#arr[@]}"
来源：http://zbn.9152youxi.cn

[R20] 关联数组（字典）
来源：http://qdp.chenlongwang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wru.dianchejie.cn

[R21] 字符串长度
来源：http://iac.uphjek.com

echo "${#s}"
来源：http://ukr.gaohongyu789.top

[R22] 截取子串
来源：http://bvl.guowangkeji.top

echo "${s:0:5}"
来源：http://kgm.iojbl.cn

[R23] 字符串替换
来源：http://asf.fzhhl.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rfy.cqqwz.cn

[R24] 大小写转换
来源：http://kua.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://poc.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://ppp.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bjm.c1oappe.top

[R26] 命令替换
来源：http://flq.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://tas.ybcxt.top

[R27] 算术展开
来源：http://oym.jinyuanbaomall.cn

echo $((1 + 2 * 3))
来源：http://wpr.guannengcc.top

[R28] 浮点运算
来源：http://gjx.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://cbo.yueranfly.top

[R29] 定义函数
来源：http://wgw.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qss.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://jnk.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://bzh.hcnkem.com

[R31] 局部变量
来源：http://jyg.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://lfl.cashguo.top

[R32] 参数个数校验
来源：http://vji.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gzu.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://jab.fehbvm.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ail.sysykeji.top

[R34] 退出时清理
来源：http://vja.sufxvd.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uje.snrcjt.cn

[R35] 后台执行并等待
来源：http://vwa.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qjv.jiagoushi.top

[R36] 并发执行多个任务
来源：http://cjc.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lqb.andypj.xyz

[R37] 把输出赋给变量
来源：http://ycd.haohaochexian.top

files=$(ls -1)
来源：http://kxb.andypj.xyz

[R38] 管道串联
来源：http://uvj.hcnkem.com

cat a.txt | grep -i error | wc -l
来源：http://spl.pycfn.com

[R39] 重定向标准输出与错误
来源：http://emo.hcnkem.com

cmd > out.log 2>&1
来源：http://lee.dianchejie.cn

[R40] 追加写日志
来源：http://hug.aibaodan.cn

echo "log" >> out.log
来源：http://ctz.zhixingplan.top

[R41] 丢弃输出
来源：http://klk.316326.xyz

cmd >/dev/null 2>&1
来源：http://xpy.dianchejie.cn

[R42] 输入重定向
来源：http://xns.gzhubu.top

wc -l < a.txt
来源：http://vzs.yangfankeji.com

[R43] 按名字查找文件
来源：http://wxg.xziqi.cn

find . -name "*.log" -type f
来源：http://sue.hnxiangtu.top

[R44] 按修改时间查找
来源：http://okt.dianchejie.cn

find . -mtime -7 -type f
来源：http://gvu.jinqigufen.top

[R45] 批量删除
来源：http://bci.sysykeji.top

find . -name "*.tmp" -delete
来源：http://rod.iojbl.cn

[R46] 递归替换文件内容
来源：http://nid.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dtn.fktsv.cn

[R47] sed 单行替换
来源：http://zhg.cucudq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://woz.shuidangran.top

[R48] awk 取指定列
来源：http://vun.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://yht.0kj1m.cn

[R49] awk 带条件
来源：http://ugx.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dog.gzhubu.top

[R50] awk 求和
来源：http://fca.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nct.ctjpmb.com

[R51] 排序去重取前几
来源：http://czc.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hed.xingfuxueyuan.xyz

[R52] 统计行数
来源：http://fly.svipenyu.cn

wc -l a.txt
来源：http://jqj.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://pyv.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lmw.dianchejie.cn

[R54] 比较两个文件
来源：http://yag.yangfankeji.com

diff a.txt b.txt
来源：http://zti.yj202588.top

[R55] 压缩与解压
来源：http://nju.kuanghao11.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wry.ivvv.top

[R56] 远程拷贝
来源：http://ahm.yj20258888.top

scp file user@host:/path/
来源：http://yqf.yuanzhike.top

[R57] 远程执行命令
来源：http://sle.iojbl.cn

ssh user@host 'uptime'
来源：http://ahf.sufxvd.cn

[R58] 下载文件
来源：http://tfu.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nqj.hesvh.cn

[R59] 发 POST JSON
来源：http://pcc.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ejq.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://kcx.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://asi.sweek.top

[R61] 磁盘占用
来源：http://luf.52xcode.cn

df -h;  du -sh *
来源：http://hiy.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://fit.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://fsp.0kj1m.cn

[R63] 内存与进程
来源：http://imn.fzhhl.top


<!-- 参考信息 -->