代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tyx.jianghu66.top

[Q20] IN 列表
来源：http://cxv.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wtb.gogol.net.cn

[Q21] 空值判断
来源：http://gdp.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://vwi.ywan-chungtsiang.top

[Q22] 排序
来源：http://dhv.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tqo.ybcxt.top

[Q23] 分页
来源：http://cqj.guowangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://udl.xuetiantiany.cn

[Q24] 去重
来源：http://jli.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://uaj.meibo888.top

[Q25] 只取前 N 条
来源：http://tsa.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eyw.tianlin.xyz

[Q26] 计数
来源：http://vxp.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://gsi.jianghu66.top

[Q27] 条件计数
来源：http://hlb.yonumen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mxo.meibo888.top

[Q28] 求和与平均
来源：http://nmc.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uhq.zhongyouzk.top

[Q29] 最大最小值
来源：http://wmb.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://erl.yj20258.top

[Q30] 分组统计
来源：http://mbe.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kpr.yonumen.top

[Q31] 分组后过滤
来源：http://nld.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://noj.yongpay.top

[Q32] 分组拼接字符串
来源：http://tyy.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ucr.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cqg.jinqigfzy.top

[Q33] 多列分组
来源：http://bvd.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jyo.yongpay.top

[Q34] 每组取第一条
来源：http://rwu.yj20258888.top

SELECT * FROM (
来源：http://smq.aibaodan.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tzx.cashguo.top

) t WHERE rn = 1;
来源：http://fsn.gaohongyu789.top

[Q35] 内连接
来源：http://pqg.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aib.gotoacloud.top

[Q36] 左连接
来源：http://abj.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mra.yuanzhike.top

[Q37] 右连接
来源：http://sba.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ofx.yj202588.top

[Q38] 全外连接（PostgreSQL）
来源：http://xzb.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ndd.zycfv.cn

[Q39] 自连接（查上下级）
来源：http://gsq.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zfx.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ehg.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://aes.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hnt.zhixingplan.top

[Q41] 多表连接
来源：http://wta.316326.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://fbk.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://oim.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://tad.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://sry.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u
来源：http://xyy.fzhhl.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sta.tianlin.xyz

[Q43] 标量子查询
来源：http://tsb.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zmr.daxiang520.top

[Q44] IN 子查询
来源：http://pga.hysaishi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://imt.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://mov.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tkh.yj20258888.top

[Q46] NOT EXISTS 判断不存在
来源：http://bkc.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ane.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://pcv.zhoulong.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jdc.guowangkeji.top

[Q48] CTE 公用表表达式
来源：http://knf.vqdsnc.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://txg.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://wqh.haohaochexian.top

[Q49] 更新单行
来源：http://uny.tian-w.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vxb.sjlbkw.cn

[Q50] 批量更新
来源：http://gds.tian-w.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rqt.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://ejy.vehdjk.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qzu.jianghu66.top

[Q52] 删除指定行
来源：http://ylg.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://sgw.zhixingplan.top

[Q53] 按条件删除
来源：http://gwq.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qlr.zhaomingkeji.xyz

[Q54] 清空表
来源：http://lkp.fktsv.cn

TRUNCATE TABLE logs;
来源：http://oap.0kj1m.cn

[Q55] 排名（并列占位）
来源：http://thq.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yzm.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://vri.fengsongda.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pdi.yonumen.top

[Q57] 行号
来源：http://aro.gaohongyu789.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bmn.sweek.top

[Q58] 累计求和
来源：http://ilo.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fkb.hammf.cn

[Q59] 分组内累计
来源：http://qzo.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pnc.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://ugy.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iyb.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cbs.daxiang520.top

[Q61] 移动平均
来源：http://kvz.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dxe.tianlin.xyz

[Q62] 分组占比
来源：http://kya.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kas.dashuyun.cn

[Q63] 开启事务
来源：http://htr.zdbjq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://unh.316326.xyz

[Q64] 提交事务
来源：http://ljs.jianghu66.top

COMMIT;
来源：http://agi.jqgufenzy.top

[Q65] 回滚事务
来源：http://pqk.sxryk.cn

ROLLBACK;
来源：http://lar.jinqigfzy.top

[Q66] 行锁查询
来源：http://oam.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ssq.fzhhl.top

[Q67] 设置隔离级别
来源：http://did.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nlq.gogol.net.cn

[Q68] 保存点
来源：http://cyt.jinqigfzy.top

SAVEPOINT sp1;
来源：http://pqq.shuidangran.top

ROLLBACK TO sp1;
来源：http://ixe.hywenlv.cn

[Q69] 查看执行计划
来源：http://xlp.sjlbkw.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rqu.yvedp.cn

[Q70] 更新统计信息
来源：http://zbn.yuanzhike.top

ANALYZE TABLE users;
来源：http://sdg.dianchejie.cn

[Q71] 查看建表语句
来源：http://kxz.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zaf.jyoumei.cn

[Q72] 查看索引
来源：http://suc.zdqjudy.top

SHOW INDEX FROM users;
来源：http://ulk.zhijiandao.cn

[Q73] 查看表状态
来源：http://icp.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dae.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://kon.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hfd.sjlbkw.cn

[Q75] 日期格式化
来源：http://kpt.jianghu66.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qze.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cjb.pengpengdd.cyou

[Q76] 按天统计
来源：http://fvh.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pxl.hammf.cn

[Q77] 时间加减
来源：http://ajf.yj202588.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tnj.jinqigufen.top

[Q78] 当前时间
来源：http://wop.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gzr.guowangkeji.top

[Q79] 字符串拼接
来源：http://yxx.wangshuangyany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ftk.tarul.cn

[Q80] 字符串截取
来源：http://dai.xziqi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mqt.ppjwa.cn

[Q81] 字符串替换
来源：http://uzx.hcnkem.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jav.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://wjb.jqgfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uih.ivvv.top

[Q83] 大小写转换
来源：http://ess.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tbe.guannengcc.top

[Q84] 去除首尾空格
来源：http://vam.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://sad.nwbrower.top

[Q85] 数值取整
来源：http://pmh.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xdb.sysykeji.top

[Q86] 读取 JSON 字段
来源：http://qhn.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vsb.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://yeu.zhoulong.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gdy.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://pao.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qqr.quarkkingdee.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oyf.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://pdf.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qng.dashuyun.cn

[Q90] 生成序号列
来源：http://syd.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cns.ctjpmb.com

================================================================================
来源：http://eho.tian-w.cn

R. Bash 专题
来源：http://dky.guannengcc.top

================================================================================
来源：http://kjf.xuetiantiany.cn

[R01] shebang 与严格模式
来源：http://rjf.andypj.xyz

#!/usr/bin/env bash
来源：http://tdo.pycfn.com

set -euo pipefail
来源：http://pho.yj20258.top

[R02] 变量赋值与使用
来源：http://tyc.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://bbk.tianlin.xyz

[R03] 只读变量
来源：http://xar.jinqigfzy.top

readonly PI=3.14
来源：http://huk.hesvh.cn

[R04] 位置参数
来源：http://aot.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kbc.jqgfzy.top

[R05] 参数默认值
来源：http://fuq.hfpthk.cn

name="${1:-default}"
来源：http://hlq.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://xkq.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zse.yuxming.cn

[R07] if 判断文件
来源：http://tlp.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rqf.jianghu66.top

[R08] 数值比较
来源：http://mja.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://buk.cucudq.cn

[R09] 字符串比较
来源：http://moj.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hgb.pengpengdd.cyou

[R10] 正则匹配
来源：http://ggg.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ewx.zhaomingkeji.xyz

[R11] case 多分支
来源：http://wdn.shanyushiyangkeji.top

case "$1" in
来源：http://acg.yuxming.cn

start) echo "启动" ;;
来源：http://qbd.jlsjyb.cn

stop)  echo "停止" ;;
来源：http://vna.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://irb.zhixingplan.top

esac
来源：http://fdt.nwbrower.top

[R12] for 遍历文件
来源：http://eng.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://jtb.fehbvm.com

[R13] for 计数循环
来源：http://fqb.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://hjc.gotoacloud.top

[R14] C 风格 for
来源：http://xnc.jinyuanbaomall.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xhq.daxiang520.top

[R15] while 逐行读文件
来源：http://css.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dwp.zycfv.cn

[R16] until 等待条件
来源：http://oms.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ovk.yvedp.cn

[R17] 数组定义与取值
来源：http://ehc.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://paz.zhixingplan.top

[R18] 遍历数组
来源：http://syk.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ayg.aizwys.cn

[R19] 数组长度
来源：http://xtm.hysaishi.cn

echo "${#arr[@]}"
来源：http://nfb.meibo888.top

[R20] 关联数组（字典）
来源：http://stx.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dao.sweek.top

[R21] 字符串长度
来源：http://srp.pycfn.com

echo "${#s}"
来源：http://her.chenzaomai.com

[R22] 截取子串
来源：http://fxv.hysaishi.cn

echo "${s:0:5}"
来源：http://kwp.haohaochexian.top

[R23] 字符串替换
来源：http://uuj.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bud.zhixingplan.top

[R24] 大小写转换
来源：http://uev.yj202588.top

echo "${s^^}"; echo "${s,,}"
来源：http://qpq.hesvh.cn

[R25] 去后缀 / 去前缀
来源：http://aed.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kne.andypj.xyz

[R26] 命令替换
来源：http://rmq.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://vhb.uphjek.com

[R27] 算术展开
来源：http://omf.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://lyp.jinghuilouyu.cn

[R28] 浮点运算
来源：http://cyz.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://hng.chenlongwang.top

[R29] 定义函数
来源：http://vwv.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://irb.jianghu66.top

[R30] 函数返回状态码
来源：http://xjh.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://huc.cdnleiting.top

[R31] 局部变量
来源：http://yfl.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://qbf.ydjk.org.cn

[R32] 参数个数校验
来源：http://hhy.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uhp.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://agv.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ndy.birdmap.top

[R34] 退出时清理
来源：http://raz.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eiu.zdbjq.cn

[R35] 后台执行并等待
来源：http://gul.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fur.zdqjudy.top

[R36] 并发执行多个任务
来源：http://yfj.chenlongwang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://umo.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://gbv.dashuyun.cn

files=$(ls -1)
来源：http://kax.0kj1m.cn

[R38] 管道串联
来源：http://nyi.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://zkh.yj202588.top

[R39] 重定向标准输出与错误
来源：http://fjd.sufxvd.cn

cmd > out.log 2>&1
来源：http://lyk.dashuyun.cn

[R40] 追加写日志
来源：http://oip.yueranfly.top

echo "log" >> out.log
来源：http://hcu.ivvv.top

[R41] 丢弃输出
来源：http://csw.316326.xyz

cmd >/dev/null 2>&1
来源：http://mqs.sjlbkw.cn

[R42] 输入重定向
来源：http://cvp.nanxinkj.top

wc -l < a.txt
来源：http://lwm.hfpthk.cn

[R43] 按名字查找文件
来源：http://oja.gotoacloud.top

find . -name "*.log" -type f
来源：http://tmu.xziqi.cn

[R44] 按修改时间查找
来源：http://yoy.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://afb.chenjidiqi.icu

[R45] 批量删除
来源：http://vek.sufxvd.cn

find . -name "*.tmp" -delete
来源：http://nrx.cqqwz.cn

[R46] 递归替换文件内容
来源：http://mjz.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zbm.yuanzhike.top

[R47] sed 单行替换
来源：http://ybv.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://enh.cheryme.top

[R48] awk 取指定列
来源：http://rwh.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://kxs.redwolf501.top

[R49] awk 带条件
来源：http://acz.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uwu.wangshuangyany.cn

[R50] awk 求和
来源：http://ymq.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://acs.zhijiandao.cn

[R51] 排序去重取前几
来源：http://xmd.hongshengwenyu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ouy.sjlbkw.cn

[R52] 统计行数
来源：http://yap.yuxming.cn

wc -l a.txt
来源：http://dqt.tanke756.top

[R53] 查看文件头与实时尾
来源：http://ufx.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mvz.zdqjudy.top

[R54] 比较两个文件
来源：http://rha.52xcode.cn

diff a.txt b.txt
来源：http://qrx.yonumen.top

[R55] 压缩与解压
来源：http://dvg.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xqu.gaohongyu789.top

[R56] 远程拷贝
来源：http://lqw.gzhubu.top

scp file user@host:/path/
来源：http://yck.yj20258888.top

[R57] 远程执行命令
来源：http://iph.hywenlv.cn

ssh user@host 'uptime'
来源：http://rbu.yj20258.top

[R58] 下载文件
来源：http://fpb.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kmh.cashguo.top

[R59] 发 POST JSON
来源：http://zjd.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gxt.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://stn.tianlin.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pds.bjfxy.top

[R61] 磁盘占用
来源：http://psr.yfazqb.com

df -h;  du -sh *
来源：http://xuy.fengsongda.top

[R62] 找最占空间的文件
来源：http://nvi.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://buj.pycfn.com

[R63] 内存与进程
来源：http://nbp.yongpay.top

free -h;  ps aux | grep nginx
来源：http://ttw.yangfankeji.com

[R64] 结束进程
来源：http://yph.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://zyj.gotoacloud.top

[R65] 查看端口占用
来源：http://kvc.cqqwz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nld.yanxiufei.cn

[R66] 定时任务
来源：http://yvf.sweek.top

crontab -e;  crontab -l
来源：http://rbd.cqqwz.cn

[R67] 生成随机十六进制串
来源：http://dhn.yongpay.top

openssl rand -hex 16
来源：http://arh.sweek.top

[R68] 计算文件校验值
来源：http://zxa.yueranfly.top

sha256sum a.txt;  md5sum a.txt
来源：http://pkw.zdqjudy.top

[R69] 生成随机密码
来源：http://yxi.cheryme.top


<!-- 参考信息 -->