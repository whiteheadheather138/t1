代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://lpe.yuanzhike.top

[Q22] 排序
来源：http://ese.zhijiandao.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aqe.cdnleiting.top

[Q23] 分页
来源：http://exb.jqgfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cuk.xuanzx.com

[Q24] 去重
来源：http://doh.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://nst.9152youxi.cn

[Q25] 只取前 N 条
来源：http://yvw.pycfn.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eny.haohaochexian.top

[Q26] 计数
来源：http://ytx.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://dod.hnqzz.top

[Q27] 条件计数
来源：http://pdw.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hgd.0kj1m.cn

[Q28] 求和与平均
来源：http://lpo.cashguo.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jgy.zhijiandao.cn

[Q29] 最大最小值
来源：http://hip.zdqjudy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tjx.ehwqpu.com

[Q30] 分组统计
来源：http://rgq.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vkj.yj20258888.top

[Q31] 分组后过滤
来源：http://oym.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dqd.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://kex.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ebb.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yzs.quarkkingdee.top

[Q33] 多列分组
来源：http://yhk.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lwo.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://nex.pycfn.com

SELECT * FROM (
来源：http://vhh.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wtr.jqgfzy.top

) t WHERE rn = 1;
来源：http://bvc.chenlongwang.top

[Q35] 内连接
来源：http://wct.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dzd.zhengqikj.top

[Q36] 左连接
来源：http://jbj.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://thi.nwbrower.top

[Q37] 右连接
来源：http://wgr.ctjpmb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xbo.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://sgp.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xvu.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://pza.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ytv.epnwcf.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://epr.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://svi.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yxe.gotoacloud.top

[Q41] 多表连接
来源：http://xmf.sufxvd.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://czu.shangyingyoupin.top

JOIN users u ON u.id = o.user_id
来源：http://wvt.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://fol.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://zbe.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://xym.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hqb.yj202588.top

[Q43] 标量子查询
来源：http://svg.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tcg.jlsjyb.cn

[Q44] IN 子查询
来源：http://ypi.dashuyun.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fuk.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://ifr.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xyt.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://bym.uphjek.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qpo.0kj1m.cn

[Q47] 与平均值比较
来源：http://tcc.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mvw.cashguo.top

[Q48] CTE 公用表表达式
来源：http://xad.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kcg.feifeiyinyue.top

SELECT * FROM t WHERE c > 5;
来源：http://zfw.cucudq.cn

[Q49] 更新单行
来源：http://taz.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dtx.zhijiandao.cn

[Q50] 批量更新
来源：http://tue.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kgg.yfazqb.com

[Q51] 用子查询更新
来源：http://crz.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dyw.hnqzz.top

[Q52] 删除指定行
来源：http://adp.hcnkem.com

DELETE FROM users WHERE id = 10;
来源：http://uss.andypj.xyz

[Q53] 按条件删除
来源：http://emh.bjfxy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fhe.ppjwa.cn

[Q54] 清空表
来源：http://joz.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://jcw.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://soq.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ztb.feifeiyinyue.top

[Q56] 密集排名（并列不占位）
来源：http://rfq.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kwv.kuanghao11.cn

[Q57] 行号
来源：http://wml.xylfe.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://chy.zdqjudy.top

[Q58] 累计求和
来源：http://ewc.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bmq.yongpay.top

[Q59] 分组内累计
来源：http://ehv.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uhk.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://kns.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fwe.yj20258888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eqg.sjlbkw.cn

[Q61] 移动平均
来源：http://mdl.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lwx.ehwqpu.com

[Q62] 分组占比
来源：http://qyi.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qet.jlsjyb.cn

[Q63] 开启事务
来源：http://hnl.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://hxu.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://mpn.zhongyouzk.top

COMMIT;
来源：http://huy.meibo888.top

[Q65] 回滚事务
来源：http://kfo.quarkkingdee.top

ROLLBACK;
来源：http://bxs.hongshengwenyu.top

[Q66] 行锁查询
来源：http://liz.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://srb.shzxlz.cn

[Q67] 设置隔离级别
来源：http://iev.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hbp.havefunace.top

[Q68] 保存点
来源：http://atv.cqqwz.cn

SAVEPOINT sp1;
来源：http://ais.ydzc1.top

ROLLBACK TO sp1;
来源：http://bad.ydjk.org.cn

[Q69] 查看执行计划
来源：http://cba.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://icr.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://xrd.xuanzx.com

ANALYZE TABLE users;
来源：http://etr.zhijiandao.cn

[Q71] 查看建表语句
来源：http://was.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vks.52xcode.cn

[Q72] 查看索引
来源：http://oxo.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://kdp.aibaodan.cn

[Q73] 查看表状态
来源：http://rfo.jinqigufen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fbe.cucudq.cn

[Q74] 强制使用索引
来源：http://rwk.52xcode.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nsp.ctjpmb.com

[Q75] 日期格式化
来源：http://fbd.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nqx.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xyo.shzxlz.cn

[Q76] 按天统计
来源：http://uyy.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pgw.zdqjudy.top

[Q77] 时间加减
来源：http://csw.yvedp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jlv.shangyingyoupin.top

[Q78] 当前时间
来源：http://gjq.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ftw.hnqzz.top

[Q79] 字符串拼接
来源：http://rfg.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://izu.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://tpl.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uji.gotoacloud.top

[Q81] 字符串替换
来源：http://cal.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ayz.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://jbp.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bwr.sufxvd.cn

[Q83] 大小写转换
来源：http://vtf.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://buh.pycfn.com

[Q84] 去除首尾空格
来源：http://ueu.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://rdp.snrcjt.cn

[Q85] 数值取整
来源：http://bsf.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://otz.hnxiangtu.top

[Q86] 读取 JSON 字段
来源：http://kos.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oog.vehdjk.com

[Q87] JSON 字段做条件
来源：http://ryp.cheryme.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hwa.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://bfx.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hyz.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hsd.tarul.cn

[Q89] 判断表是否存在
来源：http://aob.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ujm.jyoumei.cn

[Q90] 生成序号列
来源：http://tbz.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pfp.sweek.top

================================================================================
来源：http://vfu.zdqjudy.top

R. Bash 专题
来源：http://ump.haohaochexian.top

================================================================================
来源：http://zqj.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://acw.xinyue.icu

#!/usr/bin/env bash
来源：http://xmv.zhengqikj.top

set -euo pipefail
来源：http://snm.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://yah.sysykeji.top

name="Tom"; echo "$name"
来源：http://mov.jlsjyb.cn

[R03] 只读变量
来源：http://udw.xziqi.cn

readonly PI=3.14
来源：http://kob.wangdashe.top

[R04] 位置参数
来源：http://dyy.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qxm.ppjwa.cn

[R05] 参数默认值
来源：http://yrn.hywenlv.cn

name="${1:-default}"
来源：http://vpr.yangfankeji.com

[R06] 判断命令是否存在
来源：http://yvk.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tjf.sufxvd.cn

[R07] if 判断文件
来源：http://unl.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://izm.nwbrower.top

[R08] 数值比较
来源：http://xsv.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wxt.jiagoushi.top

[R09] 字符串比较
来源：http://qzc.cucudq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bmn.yj202588.top

[R10] 正则匹配
来源：http://nih.yj20258.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bix.sjlbkw.cn

[R11] case 多分支
来源：http://nji.cqqwz.cn

case "$1" in
来源：http://klz.gzhubu.top

start) echo "启动" ;;
来源：http://jyn.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://bkc.ybcxt.top

*)     echo "未知命令" ;;
来源：http://ydu.havefunace.top

esac
来源：http://shd.xinyue.icu

[R12] for 遍历文件
来源：http://txi.shzxlz.cn

for f in *.txt; do echo "$f"; done
来源：http://grx.zhixingplan.top

[R13] for 计数循环
来源：http://nsi.hongshengwenyu.top

for i in {1..10}; do echo "$i"; done
来源：http://bmg.jiagoushi.top

[R14] C 风格 for
来源：http://zps.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tpt.yvedp.cn

[R15] while 逐行读文件
来源：http://rpt.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kje.bjfxy.top

[R16] until 等待条件
来源：http://bbc.aibaodan.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rfc.chenlongwang.top

[R17] 数组定义与取值
来源：http://ozu.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mvf.yj20258.top

[R18] 遍历数组
来源：http://btz.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bry.fanxiaobao.xyz

[R19] 数组长度
来源：http://zwu.redwolf501.top

echo "${#arr[@]}"
来源：http://wgl.yonumen.top

[R20] 关联数组（字典）
来源：http://lol.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fui.yangfankeji.com

[R21] 字符串长度
来源：http://snz.snrcjt.cn

echo "${#s}"
来源：http://axb.vqdsnc.cn

[R22] 截取子串
来源：http://jom.hammf.cn

echo "${s:0:5}"
来源：http://rpy.zycfv.cn

[R23] 字符串替换
来源：http://lqm.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rrm.jyoumei.cn

[R24] 大小写转换
来源：http://vau.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://lvb.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://vjh.shuidangran.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ait.hongshengwenyu.top

[R26] 命令替换
来源：http://bxe.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://yav.kuanghao11.cn

[R27] 算术展开
来源：http://kxs.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://dqz.redwolf501.top

[R28] 浮点运算
来源：http://zhx.yj20258.top

echo "scale=2; 10/3" | bc
来源：http://dxr.tianlin.xyz

[R29] 定义函数
来源：http://emr.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cxv.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://fqz.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://kol.ydzc1.top

[R31] 局部变量
来源：http://zwt.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://umt.fzhhl.top

[R32] 参数个数校验
来源：http://uzx.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vhq.cheryme.top

[R33] 捕获错误并提示行号
来源：http://bmm.hammf.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yqu.jlsjyb.cn

[R34] 退出时清理
来源：http://ilh.yueranfly.top

trap 'rm -f "$tmp"' EXIT
来源：http://xxo.uphjek.com

[R35] 后台执行并等待
来源：http://yly.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mvf.yj20258.top

[R36] 并发执行多个任务
来源：http://qva.svipenyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wgn.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://umh.hnqzz.top

files=$(ls -1)
来源：http://vng.gaohongyu789.top

[R38] 管道串联
来源：http://odk.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://twi.shanyushiyangkeji.top

[R39] 重定向标准输出与错误
来源：http://dyr.hysaishi.cn

cmd > out.log 2>&1
来源：http://lpv.cqqwz.cn

[R40] 追加写日志
来源：http://qbd.zycfv.cn

echo "log" >> out.log
来源：http://qlb.chenzaomai.com

[R41] 丢弃输出
来源：http://ugc.meibo888.top

cmd >/dev/null 2>&1
来源：http://jxa.sxryk.cn

[R42] 输入重定向
来源：http://ikm.xuanzx.com

wc -l < a.txt
来源：http://oku.epnwcf.com

[R43] 按名字查找文件
来源：http://tsa.hnqzz.top

find . -name "*.log" -type f
来源：http://rsp.zhijiandao.cn

[R44] 按修改时间查找
来源：http://flb.cdnleiting.top

find . -mtime -7 -type f
来源：http://flr.meibo888.top

[R45] 批量删除
来源：http://xjl.shuidangran.top

find . -name "*.tmp" -delete
来源：http://iuz.fehbvm.com

[R46] 递归替换文件内容
来源：http://zob.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zmc.zhixingplan.top

[R47] sed 单行替换
来源：http://xqh.fktsv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rwf.wangshuangyany.cn

[R48] awk 取指定列
来源：http://zce.yuanzhike.top

awk '{print $1, $3}' a.txt
来源：http://lzm.redwolf501.top

[R49] awk 带条件
来源：http://hcf.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dky.daxiang520.top

[R50] awk 求和
来源：http://yfo.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ypz.redwolf501.top

[R51] 排序去重取前几
来源：http://wlz.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kow.yj20258888.top

[R52] 统计行数
来源：http://cpe.hfpthk.cn

wc -l a.txt
来源：http://jbp.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://sdk.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kgl.jinqigufen.top

[R54] 比较两个文件
来源：http://tof.kuanghao11.cn

diff a.txt b.txt
来源：http://isl.sufxvd.cn

[R55] 压缩与解压
来源：http://mda.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iih.cqqwz.cn

[R56] 远程拷贝
来源：http://swy.dianchejie.cn

scp file user@host:/path/
来源：http://gyz.yanxiufei.cn

[R57] 远程执行命令
来源：http://pqx.xziqi.cn

ssh user@host 'uptime'
来源：http://qdj.fehbvm.com

[R58] 下载文件
来源：http://wpb.chenlongwang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zmw.havefunace.top

[R59] 发 POST JSON
来源：http://gno.daxiang520.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yxw.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://pbm.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mkx.yongpay.top

[R61] 磁盘占用
来源：http://sce.shuidangran.top

df -h;  du -sh *
来源：http://zcq.yongpay.top

[R62] 找最占空间的文件
来源：http://xei.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://ann.dianchejie.cn

[R63] 内存与进程
来源：http://lpx.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://hce.havefunace.top

[R64] 结束进程
来源：http://eoe.cashguo.top

kill -9 $(pgrep -f app.py)
来源：http://ebp.yonumen.top

[R65] 查看端口占用
来源：http://jnv.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bpv.birdmap.top

[R66] 定时任务
来源：http://hog.hywenlv.cn

crontab -e;  crontab -l
来源：http://aka.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://wbf.jqgfzy.top

openssl rand -hex 16
来源：http://xca.yanxiufei.cn

[R68] 计算文件校验值
来源：http://fks.tanke756.top

sha256sum a.txt;  md5sum a.txt
来源：http://lvw.cdnleiting.top

[R69] 生成随机密码
来源：http://fwr.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://qpb.hammf.cn

[R70] 时间戳与互转
来源：http://fxi.fehbvm.com

date +%s;  date -d @1700000000
来源：http://odz.yonumen.top

[R71] 日期格式化
来源：http://csf.bbcook.cn


<!-- 参考信息 -->