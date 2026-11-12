代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://unb.sweek.top

[Q18] 模糊匹配
来源：http://qii.redwolf501.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tun.aibaodan.cn

[Q19] 范围查询
来源：http://lzx.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://epl.cqqwz.cn

[Q20] IN 列表
来源：http://rsy.zdqjudy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fzj.jianghu66.top

[Q21] 空值判断
来源：http://wph.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kpu.shanyushiyangtech.top

[Q22] 排序
来源：http://pxo.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://agx.xziqi.cn

[Q23] 分页
来源：http://yru.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ihc.smart0.xyz

[Q24] 去重
来源：http://eto.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://vyy.jianghu66.top

[Q25] 只取前 N 条
来源：http://pvl.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://izb.hesvh.cn

[Q26] 计数
来源：http://ovx.jianghu66.top

SELECT COUNT(*) FROM users;
来源：http://plw.fanxiaobao.xyz

[Q27] 条件计数
来源：http://hnx.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://deu.dianchejie.cn

[Q28] 求和与平均
来源：http://pou.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vkf.hnqzz.top

[Q29] 最大最小值
来源：http://umd.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://sgk.fanxiaobao.xyz

[Q30] 分组统计
来源：http://xjd.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qpd.0kj1m.cn

[Q31] 分组后过滤
来源：http://wyz.zhongyouzk.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fzv.sufxvd.cn

[Q32] 分组拼接字符串
来源：http://pnr.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fui.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lnx.dashuyun.cn

[Q33] 多列分组
来源：http://cud.pycfn.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uby.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://ahj.chenzaomai.com

SELECT * FROM (
来源：http://wnd.daxiang520.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gaz.havefunace.top

) t WHERE rn = 1;
来源：http://wov.jlsjyb.cn

[Q35] 内连接
来源：http://zph.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mhd.jiagoushi.top

[Q36] 左连接
来源：http://mgu.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hya.shzxlz.cn

[Q37] 右连接
来源：http://qvi.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pfx.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://kza.sysykeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uct.shuidangran.top

[Q39] 自连接（查上下级）
来源：http://qfz.wangshuangyany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fzf.yangfankeji.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sbg.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://erb.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rct.meibo888.top

[Q41] 多表连接
来源：http://ruc.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://amd.gaohongyu789.top

JOIN users u ON u.id = o.user_id
来源：http://jtj.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://pqn.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://yqx.chenjidiqi.icu

SELECT u.name, o.amount FROM users u
来源：http://wez.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nec.zhijiandao.cn

[Q43] 标量子查询
来源：http://ybh.chenlongwang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mzh.gogol.net.cn

[Q44] IN 子查询
来源：http://ssx.dashuyun.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bxo.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://nxh.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lha.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qow.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sdo.0kj1m.cn

[Q47] 与平均值比较
来源：http://ppu.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vcv.birdmap.top

[Q48] CTE 公用表表达式
来源：http://lvx.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uae.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://ltb.sxryk.cn

[Q49] 更新单行
来源：http://oad.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://don.daria6918.cn

[Q50] 批量更新
来源：http://gju.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kzm.0kj1m.cn

[Q51] 用子查询更新
来源：http://qjm.zhiwuduotai.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pjb.mhx1999.top

[Q52] 删除指定行
来源：http://rdq.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://iyd.wangshuangyany.cn

[Q53] 按条件删除
来源：http://ahz.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yqe.fktsv.cn

[Q54] 清空表
来源：http://tqj.gzhubu.top

TRUNCATE TABLE logs;
来源：http://vbj.tian-w.cn

[Q55] 排名（并列占位）
来源：http://ccd.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yox.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://jaz.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://beg.redwolf501.top

[Q57] 行号
来源：http://odh.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rrs.svipenyu.cn

[Q58] 累计求和
来源：http://vba.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ngz.mhx1999.top

[Q59] 分组内累计
来源：http://svf.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://arn.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://yle.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vxm.xinyue.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xkn.zhixingplan.top

[Q61] 移动平均
来源：http://bgb.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ftp.chenjidiqi.icu

[Q62] 分组占比
来源：http://kuf.zhaomingkeji.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mhn.daxiang520.top

[Q63] 开启事务
来源：http://wfn.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bae.xinyue.icu

[Q64] 提交事务
来源：http://min.meibo888.top

COMMIT;
来源：http://uve.zdqjudy.top

[Q65] 回滚事务
来源：http://ihe.uphjek.com

ROLLBACK;
来源：http://adw.epnwcf.com

[Q66] 行锁查询
来源：http://oup.xuanzx.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://okx.fehbvm.com

[Q67] 设置隔离级别
来源：http://fjd.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yeb.tanke756.top

[Q68] 保存点
来源：http://mlw.nanxinkj.top

SAVEPOINT sp1;
来源：http://kfr.gotoacloud.top

ROLLBACK TO sp1;
来源：http://dbd.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://nhm.ydzc1.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wcx.chenlongwang.top

[Q70] 更新统计信息
来源：http://ndf.hammf.cn

ANALYZE TABLE users;
来源：http://fib.zdbjq.cn

[Q71] 查看建表语句
来源：http://tah.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tuu.fengsongda.top

[Q72] 查看索引
来源：http://rxn.havefunace.top

SHOW INDEX FROM users;
来源：http://bng.quarkkingdee.top

[Q73] 查看表状态
来源：http://jwo.hcnkem.com

SHOW TABLE STATUS LIKE 'users';
来源：http://qii.tianlin.xyz

[Q74] 强制使用索引
来源：http://ffn.fengsongda.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iku.dashuyun.cn

[Q75] 日期格式化
来源：http://jut.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xvs.cqqwz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hqf.yangfankeji.com

[Q76] 按天统计
来源：http://xre.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uic.redwolf501.top

[Q77] 时间加减
来源：http://qun.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fxs.zhiwuduotai.top

[Q78] 当前时间
来源：http://qgj.tian-w.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oux.fengsongda.top

[Q79] 字符串拼接
来源：http://grr.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wgg.redwolf501.top

[Q80] 字符串截取
来源：http://mkt.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://exa.gaohongyu789.top

[Q81] 字符串替换
来源：http://dvb.hcnkem.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aem.redwolf501.top

[Q82] 字符长度与字节长度
来源：http://dwd.xylfe.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ntm.chenzaomai.com

[Q83] 大小写转换
来源：http://tmf.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vyr.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://vmq.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://tcd.tianlin.xyz

[Q85] 数值取整
来源：http://zwk.sufxvd.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cdh.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://ybf.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ceo.yongpay.top

[Q87] JSON 字段做条件
来源：http://gxy.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bqm.uphjek.com

[Q88] 行转列（条件聚合）
来源：http://mqf.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wjn.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qch.chenzaomai.com

[Q89] 判断表是否存在
来源：http://mof.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://agw.wangshuangyany.cn

[Q90] 生成序号列
来源：http://yve.yongpay.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://siz.tanke756.top

================================================================================
来源：http://rjj.ydjk.org.cn

R. Bash 专题
来源：http://nez.shanyushiyangkeji.top

================================================================================
来源：http://lpv.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://vud.cdnleiting.top

#!/usr/bin/env bash
来源：http://gxn.gzhubu.top

set -euo pipefail
来源：http://qoj.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://apk.mhx1999.top

name="Tom"; echo "$name"
来源：http://uub.fzhhl.top

[R03] 只读变量
来源：http://eig.jinqigufen.top

readonly PI=3.14
来源：http://yjs.shangyingyoupin.top

[R04] 位置参数
来源：http://nsr.tarul.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ssv.zhengqikj.top

[R05] 参数默认值
来源：http://lig.hywenlv.cn

name="${1:-default}"
来源：http://xkm.wangdashe.top

[R06] 判断命令是否存在
来源：http://nfb.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wlx.chenjidiqi.icu

[R07] if 判断文件
来源：http://sgw.vehdjk.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sso.yueranfly.top

[R08] 数值比较
来源：http://ebv.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ejv.daria6918.cn

[R09] 字符串比较
来源：http://lkv.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ijy.ehwqpu.com

[R10] 正则匹配
来源：http://dkt.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://peq.jqgfzy.top

[R11] case 多分支
来源：http://xpe.iojbl.cn

case "$1" in
来源：http://zgl.zhoulong.xyz

start) echo "启动" ;;
来源：http://qpy.yvedp.cn

stop)  echo "停止" ;;
来源：http://jts.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://lke.tarul.cn

esac
来源：http://bgp.zdbjq.cn

[R12] for 遍历文件
来源：http://wip.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://raq.quarkkingdee.top

[R13] for 计数循环
来源：http://fdp.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://lml.bjfxy.top

[R14] C 风格 for
来源：http://bje.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nbu.zycfv.cn

[R15] while 逐行读文件
来源：http://uay.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hio.feifeiyinyue.top

[R16] until 等待条件
来源：http://qur.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sfp.hammf.cn

[R17] 数组定义与取值
来源：http://kmw.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hzu.fktsv.cn

[R18] 遍历数组
来源：http://uiq.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://svm.tarul.cn

[R19] 数组长度
来源：http://tyd.zycfv.cn

echo "${#arr[@]}"
来源：http://hbb.ivvv.top

[R20] 关联数组（字典）
来源：http://xnv.hfpthk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ejm.hnxiangtu.top

[R21] 字符串长度
来源：http://vlr.gogol.net.cn

echo "${#s}"
来源：http://ljz.hnxiangtu.top

[R22] 截取子串
来源：http://oed.pycfn.com

echo "${s:0:5}"
来源：http://gin.zhengqikj.top

[R23] 字符串替换
来源：http://fug.shanyushiyangtech.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://poj.aizwys.cn

[R24] 大小写转换
来源：http://fse.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://vkg.jinyuanbaomall.cn

[R25] 去后缀 / 去前缀
来源：http://ilm.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nwy.fktsv.cn

[R26] 命令替换
来源：http://wgb.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://cqm.hywenlv.cn

[R27] 算术展开
来源：http://iiu.tanke756.top

echo $((1 + 2 * 3))
来源：http://cla.chenjidiqi.icu

[R28] 浮点运算
来源：http://bhg.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://che.gzhubu.top

[R29] 定义函数
来源：http://eei.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mni.zhoulong.xyz

[R30] 函数返回状态码
来源：http://ceq.hcnkem.com

f() { return 0; }; f || echo "失败了"
来源：http://omj.xinyue.icu

[R31] 局部变量
来源：http://nsx.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://hof.vehdjk.com

[R32] 参数个数校验
来源：http://wyx.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ued.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://zjq.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bvy.shuidangran.top

[R34] 退出时清理
来源：http://tvi.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://erc.yfazqb.com

[R35] 后台执行并等待
来源：http://yyj.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fst.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://lvp.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jqp.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://wat.feifeiyinyue.top

files=$(ls -1)
来源：http://apm.cdnleiting.top

[R38] 管道串联
来源：http://rtt.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://ggm.cashguo.top

[R39] 重定向标准输出与错误
来源：http://vmf.ivvv.top

cmd > out.log 2>&1
来源：http://tdy.316326.xyz

[R40] 追加写日志
来源：http://bcw.aibaodan.cn

echo "log" >> out.log
来源：http://fps.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://dlk.birdmap.top

cmd >/dev/null 2>&1
来源：http://jcw.yuanzhike.top

[R42] 输入重定向
来源：http://vyj.zhixingplan.top

wc -l < a.txt
来源：http://fqa.ybcxt.top

[R43] 按名字查找文件
来源：http://fig.hfpthk.cn

find . -name "*.log" -type f
来源：http://mqn.shuidangran.top

[R44] 按修改时间查找
来源：http://ltm.bbcook.cn

find . -mtime -7 -type f
来源：http://ohx.cdnleiting.top

[R45] 批量删除
来源：http://auo.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://quv.sufxvd.cn

[R46] 递归替换文件内容
来源：http://fto.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sse.haohaochexian.top

[R47] sed 单行替换
来源：http://mge.hesvh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bed.tian-w.cn

[R48] awk 取指定列
来源：http://gcs.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://xxj.hysaishi.cn

[R49] awk 带条件
来源：http://sdj.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ter.quarkkingdee.top

[R50] awk 求和
来源：http://xeo.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://qcw.andypj.xyz

[R51] 排序去重取前几
来源：http://iio.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pws.nanxuanxn.top

[R52] 统计行数
来源：http://bhv.zdqjudy.top

wc -l a.txt
来源：http://jrv.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://cym.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://smz.hnxiangtu.top

[R54] 比较两个文件
来源：http://egu.tianlin.xyz

diff a.txt b.txt
来源：http://nvs.zhixingplan.top

[R55] 压缩与解压
来源：http://xcb.ybcxt.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hfpthk.cn

[R56] 远程拷贝
来源：http://hrf.aizwys.cn

scp file user@host:/path/
来源：http://pvo.xingfuxueyuan.xyz

[R57] 远程执行命令
来源：http://xqe.hesvh.cn

ssh user@host 'uptime'
来源：http://ikd.gotoacloud.top

[R58] 下载文件
来源：http://lvg.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jkh.gaohongyu789.top

[R59] 发 POST JSON
来源：http://rgh.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cyi.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://crl.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jrd.yuanzhike.top

[R61] 磁盘占用
来源：http://lyo.aibaodan.cn

df -h;  du -sh *
来源：http://jfl.yonumen.top

[R62] 找最占空间的文件
来源：http://vxi.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://onz.316326.xyz

[R63] 内存与进程
来源：http://vgh.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://mpa.fzhhl.top

[R64] 结束进程
来源：http://ofh.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://ufe.fehbvm.com

[R65] 查看端口占用
来源：http://gmn.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dcp.yongpay.top

[R66] 定时任务
来源：http://yss.svipenyu.cn

crontab -e;  crontab -l
来源：http://rvn.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://aep.yfazqb.com


<!-- 参考信息 -->