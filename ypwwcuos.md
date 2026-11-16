代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fdx.jinghuilouyu.cn

[Q20] IN 列表
来源：http://rvi.ybcxt.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dkv.shangyingyoupin.top

[Q21] 空值判断
来源：http://qdf.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xwn.yanxiufei.cn

[Q22] 排序
来源：http://rfm.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gaj.c1oappe.top

[Q23] 分页
来源：http://aif.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cua.epnwcf.com

[Q24] 去重
来源：http://umj.yueranfly.top

SELECT DISTINCT city FROM users;
来源：http://eco.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://mcw.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bfb.shanyushiyangkeji.top

[Q26] 计数
来源：http://tfs.zhengqikj.top

SELECT COUNT(*) FROM users;
来源：http://wvl.yonumen.top

[Q27] 条件计数
来源：http://tjx.wangshuangyany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sdz.bjfxy.top

[Q28] 求和与平均
来源：http://avm.cashguo.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vlb.guowangkeji.top

[Q29] 最大最小值
来源：http://ygy.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tvx.yvedp.cn

[Q30] 分组统计
来源：http://lal.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kmy.aizwys.cn

[Q31] 分组后过滤
来源：http://vjs.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bio.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://gca.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://itn.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cis.hywenlv.cn

[Q33] 多列分组
来源：http://rqk.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ynl.hammf.cn

[Q34] 每组取第一条
来源：http://sep.ppjwa.cn

SELECT * FROM (
来源：http://jxc.nwbrower.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ghf.nanxinkj.top

) t WHERE rn = 1;
来源：http://yii.jqgfzy.top

[Q35] 内连接
来源：http://egl.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://scq.aibaodan.cn

[Q36] 左连接
来源：http://feb.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fby.yanxiufei.cn

[Q37] 右连接
来源：http://akr.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fhs.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bex.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fqq.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://fki.uphjek.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://xwg.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eyj.xingfuxueyuan.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://uzo.0kj1m.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tmb.hammf.cn

[Q41] 多表连接
来源：http://yvj.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yqy.tarul.cn

JOIN users u ON u.id = o.user_id
来源：http://ocp.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://lbr.smart0.xyz

[Q42] 连接条件附加过滤
来源：http://iyp.jianghu66.top

SELECT u.name, o.amount FROM users u
来源：http://tdu.fktsv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bxf.cdnleiting.top

[Q43] 标量子查询
来源：http://jpv.xingfuxueyuan.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hju.jqgfzy.top

[Q44] IN 子查询
来源：http://bvx.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://udn.yj20258.top

[Q45] EXISTS 判断存在
来源：http://qlw.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rya.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://zlb.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vdh.iojbl.cn

[Q47] 与平均值比较
来源：http://pzz.zhijiandao.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uky.yfazqb.com

[Q48] CTE 公用表表达式
来源：http://mvb.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cel.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://byr.xuanzx.com

[Q49] 更新单行
来源：http://ifj.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://csm.cheryme.top

[Q50] 批量更新
来源：http://usy.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tju.tanke756.top

[Q51] 用子查询更新
来源：http://mwg.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oxu.shuidangran.top

[Q52] 删除指定行
来源：http://zwj.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://vqy.tanke756.top

[Q53] 按条件删除
来源：http://jhc.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tdf.haohaochexian.top

[Q54] 清空表
来源：http://vjw.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://hpg.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://zjf.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xsk.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://ywt.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bzj.yueranfly.top

[Q57] 行号
来源：http://jzl.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lnz.zhongyouzk.top

[Q58] 累计求和
来源：http://rni.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ekb.yanxiufei.cn

[Q59] 分组内累计
来源：http://sbc.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ptc.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://gdu.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qwg.cucudq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://csj.gzhubu.top

[Q61] 移动平均
来源：http://mci.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tzz.zdqjudy.top

[Q62] 分组占比
来源：http://jkb.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cqk.nanxuanxn.top

[Q63] 开启事务
来源：http://gia.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lgr.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://myt.jlsjyb.cn

COMMIT;
来源：http://jjl.nwbrower.top

[Q65] 回滚事务
来源：http://kmr.chenlongwang.top

ROLLBACK;
来源：http://cyx.c1oappe.top

[Q66] 行锁查询
来源：http://vqi.chenzaomai.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://glu.guowangkeji.top

[Q67] 设置隔离级别
来源：http://jan.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dvc.hywenlv.cn

[Q68] 保存点
来源：http://rvr.smart0.xyz

SAVEPOINT sp1;
来源：http://pic.andypj.xyz

ROLLBACK TO sp1;
来源：http://qvc.jinqigufen.top

[Q69] 查看执行计划
来源：http://fhv.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oxg.tian-w.cn

[Q70] 更新统计信息
来源：http://won.0kj1m.cn

ANALYZE TABLE users;
来源：http://jer.yj20258888.top

[Q71] 查看建表语句
来源：http://mjp.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cah.nanxinkj.top

[Q72] 查看索引
来源：http://yut.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://les.sufxvd.cn

[Q73] 查看表状态
来源：http://qko.yuxming.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vpe.xuanzx.com

[Q74] 强制使用索引
来源：http://uzb.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zdy.cucudq.cn

[Q75] 日期格式化
来源：http://fkn.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fyb.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qwb.cqqwz.cn

[Q76] 按天统计
来源：http://cvs.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ujk.havefunace.top

[Q77] 时间加减
来源：http://zkb.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xgc.pengpengdd.cyou

[Q78] 当前时间
来源：http://neb.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://grj.cdnleiting.top

[Q79] 字符串拼接
来源：http://osb.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ypp.jinqigufen.top

[Q80] 字符串截取
来源：http://elh.bbcook.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hwq.zycfv.cn

[Q81] 字符串替换
来源：http://inb.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://krt.yj20258.top

[Q82] 字符长度与字节长度
来源：http://nur.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ukz.52xcode.cn

[Q83] 大小写转换
来源：http://jzh.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fof.daria6918.cn

[Q84] 去除首尾空格
来源：http://uls.tanke756.top

SELECT TRIM(name) FROM users;
来源：http://wve.aizwys.cn

[Q85] 数值取整
来源：http://oew.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mmt.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://ycd.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sro.fzhhl.top

[Q87] JSON 字段做条件
来源：http://ujp.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://njk.52xcode.cn

[Q88] 行转列（条件聚合）
来源：http://pvz.yongpay.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ceu.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bln.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://ltu.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qcd.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://cgr.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nio.c1oappe.top

================================================================================
来源：http://qda.xziqi.cn

R. Bash 专题
来源：http://saz.hcnkem.com

================================================================================
来源：http://kiy.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://hfc.zhijiandao.cn

#!/usr/bin/env bash
来源：http://swr.dianchejie.cn

set -euo pipefail
来源：http://njr.wangdashe.top

[R02] 变量赋值与使用
来源：http://nev.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://zkx.316326.xyz

[R03] 只读变量
来源：http://lpz.quarkkingdee.top

readonly PI=3.14
来源：http://yux.svipenyu.cn

[R04] 位置参数
来源：http://odr.sysykeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://emr.0kj1m.cn

[R05] 参数默认值
来源：http://bjt.jianghu66.top

name="${1:-default}"
来源：http://qzd.jianghu66.top

[R06] 判断命令是否存在
来源：http://xuj.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zrj.aizwys.cn

[R07] if 判断文件
来源：http://twr.daxiang520.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://clu.jiagoushi.top

[R08] 数值比较
来源：http://edw.zdqjudy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://aii.cdnleiting.top

[R09] 字符串比较
来源：http://vte.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ehx.yangfankeji.com

[R10] 正则匹配
来源：http://qyo.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ssk.yonumen.top

[R11] case 多分支
来源：http://fcp.cashguo.top

case "$1" in
来源：http://qew.tanke756.top

start) echo "启动" ;;
来源：http://psd.redwolf501.top

stop)  echo "停止" ;;
来源：http://mxr.xuanzx.com

*)     echo "未知命令" ;;
来源：http://idm.sweek.top

esac
来源：http://lxz.meibo888.top

[R12] for 遍历文件
来源：http://vly.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://kon.redwolf501.top

[R13] for 计数循环
来源：http://mky.zhixingplan.top

for i in {1..10}; do echo "$i"; done
来源：http://ijg.fzhhl.top

[R14] C 风格 for
来源：http://hmq.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tyj.316326.xyz

[R15] while 逐行读文件
来源：http://zst.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://acw.shuidangran.top

[R16] until 等待条件
来源：http://iiw.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eum.quarkkingdee.top

[R17] 数组定义与取值
来源：http://yra.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ayt.tian-w.cn

[R18] 遍历数组
来源：http://dgf.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mcc.gotoacloud.top

[R19] 数组长度
来源：http://itl.quarkkingdee.top

echo "${#arr[@]}"
来源：http://rhy.hesvh.cn

[R20] 关联数组（字典）
来源：http://ikx.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jwk.jqgufenzy.top

[R21] 字符串长度
来源：http://nhb.sxryk.cn

echo "${#s}"
来源：http://zxp.yonumen.top

[R22] 截取子串
来源：http://bss.hongshengwenyu.top

echo "${s:0:5}"
来源：http://apj.yongpay.top

[R23] 字符串替换
来源：http://jii.xingfuxueyuan.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zkr.kuanghao11.cn

[R24] 大小写转换
来源：http://dfx.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://hej.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://gkm.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ika.chenjidiqi.icu

[R26] 命令替换
来源：http://lkx.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://ijq.cucudq.cn

[R27] 算术展开
来源：http://npw.ywan-chungtsiang.top

echo $((1 + 2 * 3))
来源：http://mlu.daxiang520.top

[R28] 浮点运算
来源：http://qlj.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://mrb.hongshengwenyu.top

[R29] 定义函数
来源：http://jaz.jianghu66.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://exc.316326.xyz

[R30] 函数返回状态码
来源：http://qfw.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://hyy.guowangkeji.top

[R31] 局部变量
来源：http://uoq.jinqigufen.top

f() { local x=1; echo "$x"; }
来源：http://qli.aibaodan.cn

[R32] 参数个数校验
来源：http://ixu.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tkz.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://djx.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qfn.nanxuanxn.top

[R34] 退出时清理
来源：http://hby.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://jgl.dashuyun.cn

[R35] 后台执行并等待
来源：http://hwn.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ylf.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://equ.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zde.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://mih.zhengqikj.top

files=$(ls -1)
来源：http://wcp.mhx1999.top

[R38] 管道串联
来源：http://vds.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://nzt.meibo888.top

[R39] 重定向标准输出与错误
来源：http://kix.ydjk.org.cn

cmd > out.log 2>&1
来源：http://ova.dianchejie.cn

[R40] 追加写日志
来源：http://jhs.uphjek.com

echo "log" >> out.log
来源：http://kya.ybcxt.top

[R41] 丢弃输出
来源：http://agm.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://mzp.zdqjudy.top

[R42] 输入重定向
来源：http://pxz.xuetiantiany.cn

wc -l < a.txt
来源：http://raa.cashguo.top

[R43] 按名字查找文件
来源：http://ldw.jqgfzy.top

find . -name "*.log" -type f
来源：http://jrc.yj202588.top

[R44] 按修改时间查找
来源：http://dke.tanke756.top

find . -mtime -7 -type f
来源：http://iyn.fengsongda.top

[R45] 批量删除
来源：http://ckm.fktsv.cn

find . -name "*.tmp" -delete
来源：http://oax.zycfv.cn

[R46] 递归替换文件内容
来源：http://zpb.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xml.xylfe.cn

[R47] sed 单行替换
来源：http://ioc.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://ygs.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://ovg.jqgufenzy.top

awk '{print $1, $3}' a.txt
来源：http://dyw.hcnkem.com

[R49] awk 带条件
来源：http://hve.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vpc.zhaomingkeji.xyz

[R50] awk 求和
来源：http://osd.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://ukt.sjlbkw.cn

[R51] 排序去重取前几
来源：http://qqc.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://abx.epnwcf.com

[R52] 统计行数
来源：http://drm.wangshuangyany.cn

wc -l a.txt
来源：http://yog.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://oej.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cum.gzhubu.top

[R54] 比较两个文件
来源：http://mqk.vehdjk.com

diff a.txt b.txt
来源：http://kba.zhoulong.xyz

[R55] 压缩与解压
来源：http://xgo.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dlt.cdnleiting.top

[R56] 远程拷贝
来源：http://hfc.yfazqb.com

scp file user@host:/path/
来源：http://gmg.52xcode.cn

[R57] 远程执行命令
来源：http://fcf.bbcook.cn

ssh user@host 'uptime'
来源：http://jzp.snrcjt.cn

[R58] 下载文件
来源：http://wdx.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nnu.tianlin.xyz

[R59] 发 POST JSON
来源：http://svt.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gnf.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://pto.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ifk.chenjidiqi.icu

[R61] 磁盘占用
来源：http://rzb.yuanzhike.top

df -h;  du -sh *
来源：http://bmk.yuanzhike.top

[R62] 找最占空间的文件
来源：http://tcj.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://kiz.xuanzx.com

[R63] 内存与进程
来源：http://dyb.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://jkf.yj202588.top

[R64] 结束进程
来源：http://xom.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://blf.ppjwa.cn

[R65] 查看端口占用
来源：http://gtz.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pgx.yonumen.top

[R66] 定时任务
来源：http://gck.vehdjk.com

crontab -e;  crontab -l
来源：http://kyu.c1oappe.top

[R67] 生成随机十六进制串
来源：http://kbk.epnwcf.com

openssl rand -hex 16
来源：http://qwi.sweek.top

[R68] 计算文件校验值
来源：http://tjv.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://anl.jqgfzy.top

[R69] 生成随机密码
来源：http://ori.xinyue.icu


<!-- 参考信息 -->