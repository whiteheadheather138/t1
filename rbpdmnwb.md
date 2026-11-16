代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tdr.daxiang520.top

[Q11] 一次插入多行
来源：http://gsk.yonumen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zui.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://gyu.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://tvi.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qxl.gotoacloud.top

[Q13] 忽略重复插入
来源：http://jid.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://owg.shuidangran.top

[Q14] 存在则更新（upsert）
来源：http://jgm.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xzg.zhijiandao.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bnh.zycfv.cn

[Q15] 查询全部
来源：http://rkd.jiagoushi.top

SELECT * FROM users;
来源：http://fzz.gaohongyu789.top

[Q16] 查询指定列
来源：http://wmp.yj20258888.top

SELECT id, name FROM users;
来源：http://pli.yvedp.cn

[Q17] 条件查询
来源：http://xmx.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lhn.sweek.top

[Q18] 模糊匹配
来源：http://dic.sufxvd.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qqv.yuanzhike.top

[Q19] 范围查询
来源：http://wot.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qdh.yongpay.top

[Q20] IN 列表
来源：http://bzn.nanxinkj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zax.hesvh.cn

[Q21] 空值判断
来源：http://hmq.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qic.hcnkem.com

[Q22] 排序
来源：http://nrr.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vnq.feifeiyinyue.top

[Q23] 分页
来源：http://wyk.cqqwz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xmn.jinqigufen.top

[Q24] 去重
来源：http://xrm.mhx1999.top

SELECT DISTINCT city FROM users;
来源：http://pze.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://svt.cqqwz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zhh.andypj.xyz

[Q26] 计数
来源：http://ppk.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://hjq.fengsongda.top

[Q27] 条件计数
来源：http://fjo.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dun.sufxvd.cn

[Q28] 求和与平均
来源：http://fgi.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eab.zhoulong.xyz

[Q29] 最大最小值
来源：http://unc.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://ixt.daxiang520.top

[Q30] 分组统计
来源：http://sfb.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kyh.xinyue.icu

[Q31] 分组后过滤
来源：http://wbi.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ofb.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://ipc.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yhv.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://snc.hnqzz.top

[Q33] 多列分组
来源：http://zns.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fcg.xingfuxueyuan.xyz

[Q34] 每组取第一条
来源：http://hxh.xziqi.cn

SELECT * FROM (
来源：http://ypr.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rvx.svipenyu.cn

) t WHERE rn = 1;
来源：http://hog.fengsongda.top

[Q35] 内连接
来源：http://htv.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qpw.chenjidiqi.icu

[Q36] 左连接
来源：http://csp.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mdk.tian-w.cn

[Q37] 右连接
来源：http://rcb.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aid.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://cxw.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bpe.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://rig.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://iyv.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pye.zhongyouzk.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zhh.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://crf.tianlin.xyz

[Q41] 多表连接
来源：http://jad.zhiwuduotai.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yvs.gogol.net.cn

JOIN users u ON u.id = o.user_id
来源：http://vqt.zhoulong.xyz

JOIN products p ON p.id = o.product_id;
来源：http://dgu.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://glh.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://exe.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oan.cucudq.cn

[Q43] 标量子查询
来源：http://ncn.jinqigufen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jkx.wangshuangyany.cn

[Q44] IN 子查询
来源：http://gfy.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hwa.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://rgo.bbcook.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fab.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://sxm.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://deo.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://azg.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xwe.chenzaomai.com

[Q48] CTE 公用表表达式
来源：http://alv.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ckf.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://thy.xylfe.cn

[Q49] 更新单行
来源：http://lsk.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cbk.cucudq.cn

[Q50] 批量更新
来源：http://sit.yj20258888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nvc.52xcode.cn

[Q51] 用子查询更新
来源：http://hvo.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eih.ydjk.org.cn

[Q52] 删除指定行
来源：http://eev.jinqigufen.top

DELETE FROM users WHERE id = 10;
来源：http://rlj.wangdashe.top

[Q53] 按条件删除
来源：http://oll.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tgn.wangdashe.top

[Q54] 清空表
来源：http://fqk.sufxvd.cn

TRUNCATE TABLE logs;
来源：http://ykv.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://ijy.jqgfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tfj.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://fja.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://voc.shzxlz.cn

[Q57] 行号
来源：http://tji.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zzq.gogol.net.cn

[Q58] 累计求和
来源：http://lkx.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dde.ppjwa.cn

[Q59] 分组内累计
来源：http://jym.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fxh.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://ncs.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zzf.fanxiaobao.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://boc.tanke756.top

[Q61] 移动平均
来源：http://cbm.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yes.sysykeji.top

[Q62] 分组占比
来源：http://bon.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ueq.ywan-chungtsiang.top

[Q63] 开启事务
来源：http://xeh.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fym.andypj.xyz

[Q64] 提交事务
来源：http://lzr.chenzaomai.com

COMMIT;
来源：http://lwr.zhongyouzk.top

[Q65] 回滚事务
来源：http://bzi.meibo888.top

ROLLBACK;
来源：http://tqt.kuanghao11.cn

[Q66] 行锁查询
来源：http://osd.sxryk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hcd.yonumen.top

[Q67] 设置隔离级别
来源：http://hlm.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qib.shuidangran.top

[Q68] 保存点
来源：http://vap.quarkkingdee.top

SAVEPOINT sp1;
来源：http://dna.vqdsnc.cn

ROLLBACK TO sp1;
来源：http://inx.sysykeji.top

[Q69] 查看执行计划
来源：http://hfs.feifeiyinyue.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gug.xuetiantiany.cn

[Q70] 更新统计信息
来源：http://bww.nanxinkj.top

ANALYZE TABLE users;
来源：http://tur.hnxiangtu.top

[Q71] 查看建表语句
来源：http://jir.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qae.zhoulong.xyz

[Q72] 查看索引
来源：http://ebb.birdmap.top

SHOW INDEX FROM users;
来源：http://lnb.cqqwz.cn

[Q73] 查看表状态
来源：http://jru.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xrf.aibaodan.cn

[Q74] 强制使用索引
来源：http://qxu.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xga.wangdashe.top

[Q75] 日期格式化
来源：http://hkx.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eby.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xvy.chenlongwang.top

[Q76] 按天统计
来源：http://tfr.jinyuanbaomall.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://evy.ctjpmb.com

[Q77] 时间加减
来源：http://mrh.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tif.sweek.top

[Q78] 当前时间
来源：http://xaj.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ebm.redwolf501.top

[Q79] 字符串拼接
来源：http://nqa.gogol.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jql.snrcjt.cn

[Q80] 字符串截取
来源：http://inw.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zjo.ybcxt.top

[Q81] 字符串替换
来源：http://vus.havefunace.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qco.yongpay.top

[Q82] 字符长度与字节长度
来源：http://qef.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wju.yongpay.top

[Q83] 大小写转换
来源：http://xbx.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uki.quarkkingdee.top

[Q84] 去除首尾空格
来源：http://kir.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://bgr.jinqigfzy.top

[Q85] 数值取整
来源：http://tgg.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://als.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://tpu.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bak.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://kmv.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wip.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://xke.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ino.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wiy.meibo888.top

[Q89] 判断表是否存在
来源：http://afs.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fmy.tianlin.xyz

[Q90] 生成序号列
来源：http://qhc.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ljr.yangfankeji.com

================================================================================
来源：http://ekn.cashguo.top

R. Bash 专题
来源：http://qnc.jqgufenzy.top

================================================================================
来源：http://hpc.vehdjk.com

[R01] shebang 与严格模式
来源：http://ywt.hnqzz.top

#!/usr/bin/env bash
来源：http://ioz.yongpay.top

set -euo pipefail
来源：http://dsz.ybcxt.top

[R02] 变量赋值与使用
来源：http://xue.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://jqm.tian-w.cn

[R03] 只读变量
来源：http://ubg.jyoumei.cn

readonly PI=3.14
来源：http://fqf.ivvv.top

[R04] 位置参数
来源：http://bdg.xziqi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nmw.meibo888.top

[R05] 参数默认值
来源：http://ysj.zhixingplan.top

name="${1:-default}"
来源：http://esm.cashguo.top

[R06] 判断命令是否存在
来源：http://zqr.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://omr.iojbl.cn

[R07] if 判断文件
来源：http://idw.hcnkem.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cdm.fehbvm.com

[R08] 数值比较
来源：http://lsr.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nrn.tanke756.top

[R09] 字符串比较
来源：http://jcy.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wni.shanyushiyangtech.top

[R10] 正则匹配
来源：http://azg.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mof.snrcjt.cn

[R11] case 多分支
来源：http://kft.hnxiangtu.top

case "$1" in
来源：http://osy.daxiang520.top

start) echo "启动" ;;
来源：http://xbr.svipenyu.cn

stop)  echo "停止" ;;
来源：http://qou.daxiang520.top

*)     echo "未知命令" ;;
来源：http://mww.tanke756.top

esac
来源：http://ahw.yj202588.top

[R12] for 遍历文件
来源：http://ajs.dashuyun.cn

for f in *.txt; do echo "$f"; done
来源：http://xot.bjfxy.top

[R13] for 计数循环
来源：http://fco.sufxvd.cn

for i in {1..10}; do echo "$i"; done
来源：http://bfm.tanke756.top

[R14] C 风格 for
来源：http://hbv.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xea.yuxming.cn

[R15] while 逐行读文件
来源：http://bcv.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://umo.ivvv.top

[R16] until 等待条件
来源：http://ejy.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yms.birdmap.top

[R17] 数组定义与取值
来源：http://kkk.xylfe.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mqy.nanxinkj.top

[R18] 遍历数组
来源：http://lvz.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dih.nanxinkj.top

[R19] 数组长度
来源：http://boj.chenlongwang.top

echo "${#arr[@]}"
来源：http://kov.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://xfy.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zvq.jyoumei.cn

[R21] 字符串长度
来源：http://eeh.tianlin.xyz

echo "${#s}"
来源：http://cds.hfpthk.cn

[R22] 截取子串
来源：http://wqd.redwolf501.top

echo "${s:0:5}"
来源：http://hiy.jinqigfzy.top

[R23] 字符串替换
来源：http://wzo.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://swg.jiagoushi.top

[R24] 大小写转换
来源：http://ndm.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mma.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://hzx.tanke756.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://psx.fehbvm.com

[R26] 命令替换
来源：http://yde.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://dmw.ydzc1.top

[R27] 算术展开
来源：http://vtg.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://hjx.meibo888.top

[R28] 浮点运算
来源：http://ogr.9152youxi.cn

echo "scale=2; 10/3" | bc
来源：http://mfc.vehdjk.com

[R29] 定义函数
来源：http://gpr.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rot.aizwys.cn

[R30] 函数返回状态码
来源：http://wev.tarul.cn

f() { return 0; }; f || echo "失败了"
来源：http://per.c1oappe.top

[R31] 局部变量
来源：http://yhb.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://bjg.zhongyouzk.top

[R32] 参数个数校验
来源：http://tfb.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dai.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://eqh.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tnj.chenjidiqi.icu

[R34] 退出时清理
来源：http://iol.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dkg.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://cgn.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gcg.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://umi.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jbp.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://eob.wangshuangyany.cn

files=$(ls -1)
来源：http://lzw.fanxiaobao.xyz

[R38] 管道串联
来源：http://bia.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://tjt.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://cvw.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://uah.fanxiaobao.xyz

[R40] 追加写日志
来源：http://kbz.uphjek.com

echo "log" >> out.log
来源：http://wgz.haohaochexian.top

[R41] 丢弃输出
来源：http://cba.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://klq.uphjek.com

[R42] 输入重定向
来源：http://egh.yvedp.cn

wc -l < a.txt
来源：http://lds.ppjwa.cn

[R43] 按名字查找文件
来源：http://wef.yonumen.top

find . -name "*.log" -type f
来源：http://puy.yj20258.top

[R44] 按修改时间查找
来源：http://hxa.jinqigufen.top

find . -mtime -7 -type f
来源：http://jeg.yongpay.top

[R45] 批量删除
来源：http://cyp.sysykeji.top

find . -name "*.tmp" -delete
来源：http://cbi.yangfankeji.com

[R46] 递归替换文件内容
来源：http://zkg.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bhk.c1oappe.top

[R47] sed 单行替换
来源：http://atx.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vkv.gogol.net.cn

[R48] awk 取指定列
来源：http://bhe.shanyushiyangkeji.top

awk '{print $1, $3}' a.txt
来源：http://day.sysykeji.top

[R49] awk 带条件
来源：http://edk.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tle.svipenyu.cn

[R50] awk 求和
来源：http://kuu.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://zqg.yj20258888.top

[R51] 排序去重取前几
来源：http://vqx.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gdu.dianchejie.cn

[R52] 统计行数
来源：http://ojq.yj202588.top

wc -l a.txt
来源：http://sds.shanyushiyangtech.top

[R53] 查看文件头与实时尾
来源：http://uzo.smart0.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yiw.c1oappe.top

[R54] 比较两个文件
来源：http://xwt.uphjek.com

diff a.txt b.txt
来源：http://lzk.tarul.cn

[R55] 压缩与解压
来源：http://hfy.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gkx.jianghu66.top

[R56] 远程拷贝
来源：http://hwq.ivvv.top

scp file user@host:/path/
来源：http://jer.xziqi.cn

[R57] 远程执行命令
来源：http://tyb.nanxinkj.top

ssh user@host 'uptime'
来源：http://fok.svipenyu.cn

[R58] 下载文件
来源：http://umw.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://stv.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://cke.epnwcf.com


<!-- 参考信息 -->