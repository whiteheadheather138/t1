代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wvu.wangdashe.top

[Q18] 模糊匹配
来源：http://xys.ydjk.org.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rda.hysaishi.cn

[Q19] 范围查询
来源：http://kvt.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zyr.hnxiangtu.top

[Q20] IN 列表
来源：http://rps.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wjl.yuanzhike.top

[Q21] 空值判断
来源：http://msk.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://enh.sweek.top

[Q22] 排序
来源：http://hff.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jja.gogol.net.cn

[Q23] 分页
来源：http://vxu.quarkkingdee.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://stl.9152youxi.cn

[Q24] 去重
来源：http://dhu.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://dci.hongshengwenyu.top

[Q25] 只取前 N 条
来源：http://hec.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hfo.zhijiandao.cn

[Q26] 计数
来源：http://hrd.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://odz.tian-w.cn

[Q27] 条件计数
来源：http://sfv.guannengcc.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mcv.9152youxi.cn

[Q28] 求和与平均
来源：http://uat.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rho.yangfankeji.com

[Q29] 最大最小值
来源：http://wze.zdqjudy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mzo.hywenlv.cn

[Q30] 分组统计
来源：http://ufr.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://abs.yj202588.top

[Q31] 分组后过滤
来源：http://ndw.snrcjt.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nje.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://mbb.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wui.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://flw.kuanghao11.cn

[Q33] 多列分组
来源：http://wge.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bvd.jiagoushi.top

[Q34] 每组取第一条
来源：http://qvp.zhixingplan.top

SELECT * FROM (
来源：http://xvd.fanxiaobao.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pym.hnxiangtu.top

) t WHERE rn = 1;
来源：http://ini.bjfxy.top

[Q35] 内连接
来源：http://rjr.zhijiandao.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://afw.jqgfzy.top

[Q36] 左连接
来源：http://ylc.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://znq.zhiwuduotai.top

[Q37] 右连接
来源：http://sim.yanxiufei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bnu.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ldw.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rsq.tanke756.top

[Q39] 自连接（查上下级）
来源：http://htc.iojbl.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://omk.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://buh.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://opm.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wya.sxryk.cn

[Q41] 多表连接
来源：http://xbg.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://drz.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://eqp.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://loh.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://lvq.sysykeji.top

SELECT u.name, o.amount FROM users u
来源：http://jvf.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xnr.316326.xyz

[Q43] 标量子查询
来源：http://nor.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fnv.yueranfly.top

[Q44] IN 子查询
来源：http://ayy.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hmb.fehbvm.com

[Q45] EXISTS 判断存在
来源：http://hqd.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vqf.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qnu.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nrv.hnqzz.top

[Q47] 与平均值比较
来源：http://ytm.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jie.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://xqz.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kfg.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://rso.ppjwa.cn

[Q49] 更新单行
来源：http://obp.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://les.xinyue.icu

[Q50] 批量更新
来源：http://bkr.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ygd.jiagoushi.top

[Q51] 用子查询更新
来源：http://hwh.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bve.fehbvm.com

[Q52] 删除指定行
来源：http://gog.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://feu.dianchejie.cn

[Q53] 按条件删除
来源：http://eag.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kqu.chenjidiqi.icu

[Q54] 清空表
来源：http://puo.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://rhe.shanyushiyangtech.top

[Q55] 排名（并列占位）
来源：http://zto.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wtf.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://pna.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://msc.dashuyun.cn

[Q57] 行号
来源：http://axl.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mcl.ppjwa.cn

[Q58] 累计求和
来源：http://lal.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hqq.birdmap.top

[Q59] 分组内累计
来源：http://vbt.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yvi.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://kpo.vqdsnc.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wvg.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gth.hesvh.cn

[Q61] 移动平均
来源：http://uvk.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ipb.yuxming.cn

[Q62] 分组占比
来源：http://xtq.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://utj.hysaishi.cn

[Q63] 开启事务
来源：http://tpi.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gzv.jlsjyb.cn

[Q64] 提交事务
来源：http://fqi.jinqigfzy.top

COMMIT;
来源：http://shh.gotoacloud.top

[Q65] 回滚事务
来源：http://ncv.aibaodan.cn

ROLLBACK;
来源：http://upl.nanxinkj.top

[Q66] 行锁查询
来源：http://cqw.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wsa.bjfxy.top

[Q67] 设置隔离级别
来源：http://qvp.shanyushiyangtech.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rhm.hcnkem.com

[Q68] 保存点
来源：http://evo.sysykeji.top

SAVEPOINT sp1;
来源：http://cpp.jianghu66.top

ROLLBACK TO sp1;
来源：http://dnx.mhx1999.top

[Q69] 查看执行计划
来源：http://ddd.daria6918.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yfp.ehwqpu.com

[Q70] 更新统计信息
来源：http://bak.zhoulong.xyz

ANALYZE TABLE users;
来源：http://hnc.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://cmi.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qav.gzhubu.top

[Q72] 查看索引
来源：http://krp.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://lgn.zdbjq.cn

[Q73] 查看表状态
来源：http://rbu.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://llv.chenzaomai.com

[Q74] 强制使用索引
来源：http://djs.jinqigufen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qae.xziqi.cn

[Q75] 日期格式化
来源：http://vgq.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gqb.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gya.jiagoushi.top

[Q76] 按天统计
来源：http://wtk.yonumen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ueg.bbcook.cn

[Q77] 时间加减
来源：http://jpb.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vak.guowangkeji.top

[Q78] 当前时间
来源：http://jua.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iij.nanxinkj.top

[Q79] 字符串拼接
来源：http://zbe.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://veo.tian-w.cn

[Q80] 字符串截取
来源：http://whc.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://edk.hongshengwenyu.top

[Q81] 字符串替换
来源：http://esr.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kxw.vqdsnc.cn

[Q82] 字符长度与字节长度
来源：http://pjp.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yoc.redwolf501.top

[Q83] 大小写转换
来源：http://qiu.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://brn.yueranfly.top

[Q84] 去除首尾空格
来源：http://psx.xylfe.cn

SELECT TRIM(name) FROM users;
来源：http://gkm.uphjek.com

[Q85] 数值取整
来源：http://kuz.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fwz.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://nri.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rtb.fehbvm.com

[Q87] JSON 字段做条件
来源：http://yqh.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ray.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://ufo.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qif.guannengcc.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yus.jqgfzy.top

[Q89] 判断表是否存在
来源：http://pef.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vwu.daxiang520.top

[Q90] 生成序号列
来源：http://fyh.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tyh.tarul.cn

================================================================================
来源：http://ltb.shuidangran.top

R. Bash 专题
来源：http://hlm.hfpthk.cn

================================================================================
来源：http://dxj.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://nmm.daria6918.cn

#!/usr/bin/env bash
来源：http://kbd.fanxiaobao.xyz

set -euo pipefail
来源：http://yju.hammf.cn

[R02] 变量赋值与使用
来源：http://uzd.fehbvm.com

name="Tom"; echo "$name"
来源：http://mub.hfpthk.cn

[R03] 只读变量
来源：http://hva.jinghuilouyu.cn

readonly PI=3.14
来源：http://yxw.yongpay.top

[R04] 位置参数
来源：http://fxz.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ids.quarkkingdee.top

[R05] 参数默认值
来源：http://efb.epnwcf.com

name="${1:-default}"
来源：http://xkb.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://guz.0kj1m.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hal.tanke756.top

[R07] if 判断文件
来源：http://hgm.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://riq.redwolf501.top

[R08] 数值比较
来源：http://kxs.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://imb.bbcook.cn

[R09] 字符串比较
来源：http://zan.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qim.c1oappe.top

[R10] 正则匹配
来源：http://msr.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vwk.yj20258888.top

[R11] case 多分支
来源：http://sfh.xziqi.cn

case "$1" in
来源：http://cjz.iojbl.cn

start) echo "启动" ;;
来源：http://xas.birdmap.top

stop)  echo "停止" ;;
来源：http://bez.yj20258.top

*)     echo "未知命令" ;;
来源：http://jzh.nanxinkj.top

esac
来源：http://jnv.snrcjt.cn

[R12] for 遍历文件
来源：http://rom.ydzc1.top

for f in *.txt; do echo "$f"; done
来源：http://vzr.yongpay.top

[R13] for 计数循环
来源：http://wcy.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://noy.iojbl.cn

[R14] C 风格 for
来源：http://jso.zhoulong.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eha.fehbvm.com

[R15] while 逐行读文件
来源：http://jss.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://puf.pengpengdd.cyou

[R16] until 等待条件
来源：http://ogf.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pru.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://gpn.gotoacloud.top

arr=(a b c); echo "${arr[0]}"
来源：http://bpd.hnxiangtu.top

[R18] 遍历数组
来源：http://ptx.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aeh.fanxiaobao.xyz

[R19] 数组长度
来源：http://dwx.tanke756.top

echo "${#arr[@]}"
来源：http://zxi.ppjwa.cn

[R20] 关联数组（字典）
来源：http://dzw.ydzc1.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hrm.yuanzhike.top

[R21] 字符串长度
来源：http://cfb.wangdashe.top

echo "${#s}"
来源：http://kjz.gotoacloud.top

[R22] 截取子串
来源：http://acl.52xcode.cn

echo "${s:0:5}"
来源：http://ucc.chenlongwang.top

[R23] 字符串替换
来源：http://lkn.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ytq.nwbrower.top

[R24] 大小写转换
来源：http://yks.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ses.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://bhs.daria6918.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://slq.jinyuanbaomall.cn

[R26] 命令替换
来源：http://yqu.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://sxm.sjlbkw.cn

[R27] 算术展开
来源：http://kww.ybcxt.top

echo $((1 + 2 * 3))
来源：http://ymh.yuanzhike.top

[R28] 浮点运算
来源：http://uyp.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://ibf.shzxlz.cn

[R29] 定义函数
来源：http://uuv.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xam.52xcode.cn

[R30] 函数返回状态码
来源：http://wfg.52xcode.cn

f() { return 0; }; f || echo "失败了"
来源：http://ffv.jqgufenzy.top

[R31] 局部变量
来源：http://mlz.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://iod.guowangkeji.top

[R32] 参数个数校验
来源：http://akk.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ecl.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://sqj.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xxo.jlsjyb.cn

[R34] 退出时清理
来源：http://twc.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://vcd.yj202588.top

[R35] 后台执行并等待
来源：http://fvf.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bnk.xuanzx.com

[R36] 并发执行多个任务
来源：http://dle.fehbvm.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gzw.meibo888.top

[R37] 把输出赋给变量
来源：http://unu.guowangkeji.top

files=$(ls -1)
来源：http://ngv.tianlin.xyz

[R38] 管道串联
来源：http://emi.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://vvo.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://fcj.gaohongyu789.top

cmd > out.log 2>&1
来源：http://jod.fehbvm.com

[R40] 追加写日志
来源：http://gwr.aibaodan.cn

echo "log" >> out.log
来源：http://tjl.hysaishi.cn

[R41] 丢弃输出
来源：http://gzo.zycfv.cn

cmd >/dev/null 2>&1
来源：http://vzl.hywenlv.cn

[R42] 输入重定向
来源：http://qbz.birdmap.top

wc -l < a.txt
来源：http://pkr.meibo888.top

[R43] 按名字查找文件
来源：http://urf.zdqjudy.top

find . -name "*.log" -type f
来源：http://mlg.cashguo.top

[R44] 按修改时间查找
来源：http://iuh.zycfv.cn

find . -mtime -7 -type f
来源：http://bda.jinghuilouyu.cn

[R45] 批量删除
来源：http://ejw.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://ijo.cheryme.top

[R46] 递归替换文件内容
来源：http://xmv.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rks.yj202588.top

[R47] sed 单行替换
来源：http://mvg.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://kgf.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://luf.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://kwd.tarul.cn

[R49] awk 带条件
来源：http://tvx.fengsongda.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://swu.kuanghao11.cn

[R50] awk 求和
来源：http://rts.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kgk.cdnleiting.top

[R51] 排序去重取前几
来源：http://ndn.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ugl.yonumen.top

[R52] 统计行数
来源：http://lpp.jyoumei.cn

wc -l a.txt
来源：http://ytc.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://ygu.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oee.gotoacloud.top

[R54] 比较两个文件
来源：http://jol.yj20258888.top

diff a.txt b.txt
来源：http://kip.redwolf501.top

[R55] 压缩与解压
来源：http://hcp.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bdq.birdmap.top

[R56] 远程拷贝
来源：http://zwl.pengpengdd.cyou

scp file user@host:/path/
来源：http://vzs.vehdjk.com

[R57] 远程执行命令
来源：http://hux.ehwqpu.com

ssh user@host 'uptime'
来源：http://mzx.zhoulong.xyz

[R58] 下载文件
来源：http://lre.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qyg.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://lll.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nwf.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://zbb.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://whd.cdnleiting.top

[R61] 磁盘占用
来源：http://ire.uphjek.com

df -h;  du -sh *
来源：http://jzf.jqgufenzy.top

[R62] 找最占空间的文件
来源：http://ebp.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://tho.zycfv.cn

[R63] 内存与进程
来源：http://bkq.havefunace.top

free -h;  ps aux | grep nginx
来源：http://ofr.sweek.top

[R64] 结束进程
来源：http://swb.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://wyl.haohaochexian.top

[R65] 查看端口占用
来源：http://aqd.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://obu.yuanzhike.top

[R66] 定时任务
来源：http://aid.c1oappe.top

crontab -e;  crontab -l
来源：http://itd.cheryme.top

[R67] 生成随机十六进制串
来源：http://hbv.cdnleiting.top


<!-- 参考信息 -->