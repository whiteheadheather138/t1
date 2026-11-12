代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zbi.haohaochexian.top

[Q20] IN 列表
来源：http://vgm.pengpengdd.cyou

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://adp.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://irj.epnwcf.com

SELECT * FROM users WHERE email IS NULL;
来源：http://fji.0kj1m.cn

[Q22] 排序
来源：http://rnh.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://azd.jlsjyb.cn

[Q23] 分页
来源：http://zaf.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wmc.316326.xyz

[Q24] 去重
来源：http://tcu.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://ywn.wangdashe.top

[Q25] 只取前 N 条
来源：http://nnq.bbcook.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tye.9152youxi.cn

[Q26] 计数
来源：http://nyg.sweek.top

SELECT COUNT(*) FROM users;
来源：http://qkz.yj20258.top

[Q27] 条件计数
来源：http://omn.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dme.cashguo.top

[Q28] 求和与平均
来源：http://mre.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mij.xuanzx.com

[Q29] 最大最小值
来源：http://krl.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://cxb.xziqi.cn

[Q30] 分组统计
来源：http://gsz.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ooa.yj20258888.top

[Q31] 分组后过滤
来源：http://uan.yueranfly.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mew.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://cyz.quarkkingdee.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bsr.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hsl.hnqzz.top

[Q33] 多列分组
来源：http://vhl.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dcd.0kj1m.cn

[Q34] 每组取第一条
来源：http://bzq.vehdjk.com

SELECT * FROM (
来源：http://nwd.0kj1m.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://scq.zhoulong.xyz

) t WHERE rn = 1;
来源：http://bvd.snrcjt.cn

[Q35] 内连接
来源：http://vxn.zhoulong.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jih.ivvv.top

[Q36] 左连接
来源：http://ttw.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ewq.uphjek.com

[Q37] 右连接
来源：http://sdl.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wwy.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rnd.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fbw.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://can.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://iqy.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jsu.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dvv.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qyj.epnwcf.com

[Q41] 多表连接
来源：http://pem.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ral.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://yyp.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://sja.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://mmf.yongpay.top

SELECT u.name, o.amount FROM users u
来源：http://zfj.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zsc.hongshengwenyu.top

[Q43] 标量子查询
来源：http://huw.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lgu.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://msl.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ylr.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://dpm.hongshengwenyu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sku.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://jnc.zhoulong.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://usn.uphjek.com

[Q47] 与平均值比较
来源：http://wsz.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vkz.jinqigfzy.top

[Q48] CTE 公用表表达式
来源：http://ihn.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kod.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://hnl.yvedp.cn

[Q49] 更新单行
来源：http://dlw.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bzf.gaohongyu789.top

[Q50] 批量更新
来源：http://fhw.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xeh.aizwys.cn

[Q51] 用子查询更新
来源：http://sbu.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ivu.quarkkingdee.top

[Q52] 删除指定行
来源：http://nln.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://ddn.cheryme.top

[Q53] 按条件删除
来源：http://wjy.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qmv.zycfv.cn

[Q54] 清空表
来源：http://tbl.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://fgr.bbcook.cn

[Q55] 排名（并列占位）
来源：http://blc.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ucz.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://dqm.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yau.quarkkingdee.top

[Q57] 行号
来源：http://xtz.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jtb.wangdashe.top

[Q58] 累计求和
来源：http://xnc.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://evx.tanke756.top

[Q59] 分组内累计
来源：http://qrm.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://okg.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://mpr.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gyi.zdbjq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vln.cheryme.top

[Q61] 移动平均
来源：http://pxr.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ipw.sjlbkw.cn

[Q62] 分组占比
来源：http://vmv.feifeiyinyue.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zoi.xinyue.icu

[Q63] 开启事务
来源：http://bap.tianlin.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://pua.cucudq.cn

[Q64] 提交事务
来源：http://wlu.tian-w.cn

COMMIT;
来源：http://fbq.sufxvd.cn

[Q65] 回滚事务
来源：http://wfw.jqgufenzy.top

ROLLBACK;
来源：http://bhh.xuetiantiany.cn

[Q66] 行锁查询
来源：http://kro.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cvf.fengsongda.top

[Q67] 设置隔离级别
来源：http://gwv.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cse.zhengqikj.top

[Q68] 保存点
来源：http://bko.dianchejie.cn

SAVEPOINT sp1;
来源：http://kqc.shuidangran.top

ROLLBACK TO sp1;
来源：http://bgr.jlsjyb.cn

[Q69] 查看执行计划
来源：http://kwm.cqqwz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ecz.gotoacloud.top

[Q70] 更新统计信息
来源：http://xeb.zdbjq.cn

ANALYZE TABLE users;
来源：http://wma.gotoacloud.top

[Q71] 查看建表语句
来源：http://ets.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hnr.daxiang520.top

[Q72] 查看索引
来源：http://qra.hysaishi.cn

SHOW INDEX FROM users;
来源：http://tpo.wangshuangyany.cn

[Q73] 查看表状态
来源：http://zix.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ypq.ivvv.top

[Q74] 强制使用索引
来源：http://lpb.hywenlv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yvl.fzhhl.top

[Q75] 日期格式化
来源：http://yhq.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zub.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jmq.dashuyun.cn

[Q76] 按天统计
来源：http://egx.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wxh.zhijiandao.cn

[Q77] 时间加减
来源：http://wqu.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://quu.feifeiyinyue.top

[Q78] 当前时间
来源：http://emy.xuetiantiany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tvk.ydzc1.top

[Q79] 字符串拼接
来源：http://cih.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mkg.yonumen.top

[Q80] 字符串截取
来源：http://hyg.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://prh.andypj.xyz

[Q81] 字符串替换
来源：http://fyp.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rvi.zdbjq.cn

[Q82] 字符长度与字节长度
来源：http://udd.yongpay.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kcq.yfazqb.com

[Q83] 大小写转换
来源：http://oom.nanxuanxn.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ykb.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://muu.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://xpv.zycfv.cn

[Q85] 数值取整
来源：http://cmq.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vca.smart0.xyz

[Q86] 读取 JSON 字段
来源：http://xnx.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qkj.9152youxi.cn

[Q87] JSON 字段做条件
来源：http://uwa.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vuq.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://rks.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rvq.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://adv.fehbvm.com

[Q89] 判断表是否存在
来源：http://dwx.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://epu.pycfn.com

[Q90] 生成序号列
来源：http://wth.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ffa.pengpengdd.cyou

================================================================================
来源：http://kfx.zdbjq.cn

R. Bash 专题
来源：http://aca.jianghu66.top

================================================================================
来源：http://jaq.9152youxi.cn

[R01] shebang 与严格模式
来源：http://jid.yuanzhike.top

#!/usr/bin/env bash
来源：http://xkb.ppjwa.cn

set -euo pipefail
来源：http://uwk.sweek.top

[R02] 变量赋值与使用
来源：http://sut.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://eqc.zhongyouzk.top

[R03] 只读变量
来源：http://cyt.zdbjq.cn

readonly PI=3.14
来源：http://kmy.52xcode.cn

[R04] 位置参数
来源：http://sae.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nco.gotoacloud.top

[R05] 参数默认值
来源：http://ioo.jinqigufen.top

name="${1:-default}"
来源：http://owk.tianlin.xyz

[R06] 判断命令是否存在
来源：http://zls.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wlh.0kj1m.cn

[R07] if 判断文件
来源：http://dvb.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xqu.jinyuanbaomall.cn

[R08] 数值比较
来源：http://axw.yvedp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://emy.xinyue.icu

[R09] 字符串比较
来源：http://jkd.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gal.gotoacloud.top

[R10] 正则匹配
来源：http://uln.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cvd.jqgfzy.top

[R11] case 多分支
来源：http://ala.xylfe.cn

case "$1" in
来源：http://txd.kuanghao11.cn

start) echo "启动" ;;
来源：http://rsh.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://iza.hammf.cn

*)     echo "未知命令" ;;
来源：http://dwr.yonumen.top

esac
来源：http://ygq.zdbjq.cn

[R12] for 遍历文件
来源：http://sfc.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://kzi.yj202588.top

[R13] for 计数循环
来源：http://rpa.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://oxz.guannengcc.top

[R14] C 风格 for
来源：http://tqc.yangfankeji.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pwq.jqgufenzy.top

[R15] while 逐行读文件
来源：http://bwu.ppjwa.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dap.wangshuangyany.cn

[R16] until 等待条件
来源：http://lsz.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tlc.hnxiangtu.top

[R17] 数组定义与取值
来源：http://imf.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dla.jyoumei.cn

[R18] 遍历数组
来源：http://vnv.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qzf.c1oappe.top

[R19] 数组长度
来源：http://cby.birdmap.top

echo "${#arr[@]}"
来源：http://mvy.tarul.cn

[R20] 关联数组（字典）
来源：http://ugk.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hpn.zhiwuduotai.top

[R21] 字符串长度
来源：http://zkd.fengsongda.top

echo "${#s}"
来源：http://irm.hfpthk.cn

[R22] 截取子串
来源：http://hcv.sxryk.cn

echo "${s:0:5}"
来源：http://aae.yongpay.top

[R23] 字符串替换
来源：http://das.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kmp.daxiang520.top

[R24] 大小写转换
来源：http://rds.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://jvc.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://jsy.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tun.gogol.net.cn

[R26] 命令替换
来源：http://ekc.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://pvv.mhx1999.top

[R27] 算术展开
来源：http://vbc.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://oqv.jlsjyb.cn

[R28] 浮点运算
来源：http://gbb.ppjwa.cn

echo "scale=2; 10/3" | bc
来源：http://ckh.chenzaomai.com

[R29] 定义函数
来源：http://pnh.cdnleiting.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ujy.xylfe.cn

[R30] 函数返回状态码
来源：http://isk.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://oid.hysaishi.cn

[R31] 局部变量
来源：http://qiu.gogol.net.cn

f() { local x=1; echo "$x"; }
来源：http://gsc.snrcjt.cn

[R32] 参数个数校验
来源：http://zml.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://usf.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://tpl.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gzp.316326.xyz

[R34] 退出时清理
来源：http://ggg.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://nii.zhoulong.xyz

[R35] 后台执行并等待
来源：http://gru.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rpg.sufxvd.cn

[R36] 并发执行多个任务
来源：http://ulp.xinyue.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zac.yonumen.top

[R37] 把输出赋给变量
来源：http://ymd.xuanzx.com

files=$(ls -1)
来源：http://vhv.tian-w.cn

[R38] 管道串联
来源：http://euf.jqgfzy.top

cat a.txt | grep -i error | wc -l
来源：http://lku.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://rrb.hesvh.cn

cmd > out.log 2>&1
来源：http://zgc.ppjwa.cn

[R40] 追加写日志
来源：http://ost.sjlbkw.cn

echo "log" >> out.log
来源：http://bji.nanxinkj.top

[R41] 丢弃输出
来源：http://mom.yj202588.top

cmd >/dev/null 2>&1
来源：http://ygl.shangyingyoupin.top

[R42] 输入重定向
来源：http://hux.hywenlv.cn

wc -l < a.txt
来源：http://qvv.chenzaomai.com

[R43] 按名字查找文件
来源：http://yto.shuidangran.top

find . -name "*.log" -type f
来源：http://djr.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://cav.ydzc1.top

find . -mtime -7 -type f
来源：http://qby.yvedp.cn

[R45] 批量删除
来源：http://jhc.52xcode.cn

find . -name "*.tmp" -delete
来源：http://aal.yvedp.cn

[R46] 递归替换文件内容
来源：http://zqn.yuxming.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://prl.bjfxy.top

[R47] sed 单行替换
来源：http://nql.hnqzz.top

sed -i 's/foo/bar/g' a.txt
来源：http://ibj.gotoacloud.top

[R48] awk 取指定列
来源：http://njo.nwbrower.top

awk '{print $1, $3}' a.txt
来源：http://gja.yvedp.cn

[R49] awk 带条件
来源：http://tkd.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://npv.jinqigufen.top

[R50] awk 求和
来源：http://swp.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://tqo.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://rws.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://srb.hammf.cn

[R52] 统计行数
来源：http://gle.wangshuangyany.cn

wc -l a.txt
来源：http://ibm.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://edo.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qma.yvedp.cn

[R54] 比较两个文件
来源：http://ulv.tian-w.cn

diff a.txt b.txt
来源：http://ghl.9152youxi.cn

[R55] 压缩与解压
来源：http://lpo.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mqg.sysykeji.top

[R56] 远程拷贝
来源：http://jjb.cucudq.cn

scp file user@host:/path/
来源：http://dyv.yanxiufei.cn

[R57] 远程执行命令
来源：http://fuw.smart0.xyz

ssh user@host 'uptime'
来源：http://zko.hcnkem.com

[R58] 下载文件
来源：http://itb.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vhd.yangfankeji.com

[R59] 发 POST JSON
来源：http://iwk.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gnk.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://yzb.yuanzhike.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gxw.iojbl.cn

[R61] 磁盘占用
来源：http://qer.316326.xyz

df -h;  du -sh *
来源：http://pqt.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://xuu.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://gog.svipenyu.cn

[R63] 内存与进程
来源：http://xhh.yj20258.top

free -h;  ps aux | grep nginx
来源：http://baj.zycfv.cn

[R64] 结束进程
来源：http://siy.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://zfb.yangfankeji.com

[R65] 查看端口占用
来源：http://ios.gzhubu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://inx.xuetiantiany.cn

[R66] 定时任务
来源：http://myu.birdmap.top

crontab -e;  crontab -l
来源：http://rut.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://tsp.feifeiyinyue.top

openssl rand -hex 16
来源：http://ibc.yanxiufei.cn

[R68] 计算文件校验值
来源：http://jlp.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://psw.haohaochexian.top

[R69] 生成随机密码
来源：http://bta.tarul.cn


<!-- 参考信息 -->