代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jeg.xinyue.icu

[Q26] 计数
来源：http://zqf.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://qwr.tian-w.cn

[Q27] 条件计数
来源：http://ogg.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ldj.hesvh.cn

[Q28] 求和与平均
来源：http://xfb.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://egv.ydjk.org.cn

[Q29] 最大最小值
来源：http://cyi.cdnleiting.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bps.shzxlz.cn

[Q30] 分组统计
来源：http://ooy.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mmy.jiagoushi.top

[Q31] 分组后过滤
来源：http://ahu.tianlin.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qrw.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://kcq.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oir.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jgz.cashguo.top

[Q33] 多列分组
来源：http://mou.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xyg.snrcjt.cn

[Q34] 每组取第一条
来源：http://csq.tianlin.xyz

SELECT * FROM (
来源：http://zrv.yuxming.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://urn.nwbrower.top

) t WHERE rn = 1;
来源：http://agb.ctjpmb.com

[Q35] 内连接
来源：http://egm.fehbvm.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vaa.jqgufenzy.top

[Q36] 左连接
来源：http://fbq.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://diy.nwbrower.top

[Q37] 右连接
来源：http://imn.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hcr.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://wcb.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nlf.zdqjudy.top

[Q39] 自连接（查上下级）
来源：http://mtm.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dyl.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kvm.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://omt.haohaochexian.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zty.316326.xyz

[Q41] 多表连接
来源：http://chh.yangfankeji.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://igl.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://boo.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://dmb.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://aor.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://qon.yj20258888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zyc.jiagoushi.top

[Q43] 标量子查询
来源：http://dwx.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ixb.zycfv.cn

[Q44] IN 子查询
来源：http://jok.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oha.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://byr.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hsd.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uwp.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rao.ydzc1.top

[Q47] 与平均值比较
来源：http://exm.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sex.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://jxw.bbcook.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jev.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://pvb.zhengqikj.top

[Q49] 更新单行
来源：http://snn.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ril.meibo888.top

[Q50] 批量更新
来源：http://xhm.tianlin.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qnk.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://wij.sweek.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dvj.jlsjyb.cn

[Q52] 删除指定行
来源：http://cmp.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://cjf.gotoacloud.top

[Q53] 按条件删除
来源：http://ahk.sxryk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bwj.cqqwz.cn

[Q54] 清空表
来源：http://cse.c1oappe.top

TRUNCATE TABLE logs;
来源：http://zov.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://klc.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fwu.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://dwm.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ioo.vehdjk.com

[Q57] 行号
来源：http://hzu.uphjek.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qss.dianchejie.cn

[Q58] 累计求和
来源：http://afg.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dfi.yj20258888.top

[Q59] 分组内累计
来源：http://xqo.vehdjk.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://imp.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://bay.chenjidiqi.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hzf.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ltd.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://wkn.xziqi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nfa.haohaochexian.top

[Q62] 分组占比
来源：http://pwt.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://puc.vehdjk.com

[Q63] 开启事务
来源：http://aqq.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fbw.tian-w.cn

[Q64] 提交事务
来源：http://lyf.zhixingplan.top

COMMIT;
来源：http://lkl.cashguo.top

[Q65] 回滚事务
来源：http://tyz.cucudq.cn

ROLLBACK;
来源：http://txr.jinqigfzy.top

[Q66] 行锁查询
来源：http://kui.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tam.daria6918.cn

[Q67] 设置隔离级别
来源：http://gof.zhoulong.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wpi.fanxiaobao.xyz

[Q68] 保存点
来源：http://lvc.chenjidiqi.icu

SAVEPOINT sp1;
来源：http://kyn.hammf.cn

ROLLBACK TO sp1;
来源：http://gph.uphjek.com

[Q69] 查看执行计划
来源：http://brk.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ozg.jinqigufen.top

[Q70] 更新统计信息
来源：http://gpx.xuanzx.com

ANALYZE TABLE users;
来源：http://uhf.chenzaomai.com

[Q71] 查看建表语句
来源：http://rtn.zycfv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mwp.hnqzz.top

[Q72] 查看索引
来源：http://zep.xylfe.cn

SHOW INDEX FROM users;
来源：http://xyb.ppjwa.cn

[Q73] 查看表状态
来源：http://arp.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jwc.0kj1m.cn

[Q74] 强制使用索引
来源：http://mzo.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nex.hcnkem.com

[Q75] 日期格式化
来源：http://miv.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hjt.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://czj.yuanzhike.top

[Q76] 按天统计
来源：http://unj.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vad.yvedp.cn

[Q77] 时间加减
来源：http://hec.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bxl.zhiwuduotai.top

[Q78] 当前时间
来源：http://gch.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rbe.hammf.cn

[Q79] 字符串拼接
来源：http://csf.jianghu66.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vbn.ybcxt.top

[Q80] 字符串截取
来源：http://zcy.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gdp.kuanghao11.cn

[Q81] 字符串替换
来源：http://mdt.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bjn.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://rya.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xes.aizwys.cn

[Q83] 大小写转换
来源：http://raz.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wan.jqgfzy.top

[Q84] 去除首尾空格
来源：http://wnu.svipenyu.cn

SELECT TRIM(name) FROM users;
来源：http://ygb.316326.xyz

[Q85] 数值取整
来源：http://wcc.zdqjudy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wjg.shanyushiyangtech.top

[Q86] 读取 JSON 字段
来源：http://lta.yangfankeji.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bnr.yj20258.top

[Q87] JSON 字段做条件
来源：http://dci.zhoulong.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ywy.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://uhm.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kwt.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qlm.hfpthk.cn

[Q89] 判断表是否存在
来源：http://vpj.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cjh.ppjwa.cn

[Q90] 生成序号列
来源：http://jla.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yjo.zhongyouzk.top

================================================================================
来源：http://axc.ydjk.org.cn

R. Bash 专题
来源：http://vnm.uphjek.com

================================================================================
来源：http://sqf.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://aor.ctjpmb.com

#!/usr/bin/env bash
来源：http://mqu.zhaomingkeji.xyz

set -euo pipefail
来源：http://tjb.cashguo.top

[R02] 变量赋值与使用
来源：http://bnv.kuanghao11.cn

name="Tom"; echo "$name"
来源：http://vwc.xuanzx.com

[R03] 只读变量
来源：http://ghi.jyoumei.cn

readonly PI=3.14
来源：http://fii.meibo888.top

[R04] 位置参数
来源：http://tja.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kun.ivvv.top

[R05] 参数默认值
来源：http://aid.bbcook.cn

name="${1:-default}"
来源：http://lqu.cqqwz.cn

[R06] 判断命令是否存在
来源：http://xec.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qtv.cashguo.top

[R07] if 判断文件
来源：http://kdn.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xex.andypj.xyz

[R08] 数值比较
来源：http://vnv.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://dmk.chenzaomai.com

[R09] 字符串比较
来源：http://ali.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nqr.hongshengwenyu.top

[R10] 正则匹配
来源：http://ayi.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bds.bjfxy.top

[R11] case 多分支
来源：http://yho.zycfv.cn

case "$1" in
来源：http://iba.zhixingplan.top

start) echo "启动" ;;
来源：http://mwi.gzhubu.top

stop)  echo "停止" ;;
来源：http://mvz.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://lab.gzhubu.top

esac
来源：http://cya.meibo888.top

[R12] for 遍历文件
来源：http://wdf.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://cny.nanxuanxn.top

[R13] for 计数循环
来源：http://cmq.hongshengwenyu.top

for i in {1..10}; do echo "$i"; done
来源：http://yuf.hfpthk.cn

[R14] C 风格 for
来源：http://iry.fktsv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eyn.fzhhl.top

[R15] while 逐行读文件
来源：http://hul.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ntk.ctjpmb.com

[R16] until 等待条件
来源：http://wfn.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://heo.tianlin.xyz

[R17] 数组定义与取值
来源：http://rkl.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://ugo.yueranfly.top

[R18] 遍历数组
来源：http://tug.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uhd.ehwqpu.com

[R19] 数组长度
来源：http://vdq.shzxlz.cn

echo "${#arr[@]}"
来源：http://ktx.zhixingplan.top

[R20] 关联数组（字典）
来源：http://nfn.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bcm.jinqigfzy.top

[R21] 字符串长度
来源：http://syf.meibo888.top

echo "${#s}"
来源：http://zuz.xuetiantiany.cn

[R22] 截取子串
来源：http://fca.daxiang520.top

echo "${s:0:5}"
来源：http://ozu.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://tkd.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kxt.daxiang520.top

[R24] 大小写转换
来源：http://hft.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://pqe.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://dgm.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://iej.nanxinkj.top

[R26] 命令替换
来源：http://buj.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://rim.fehbvm.com

[R27] 算术展开
来源：http://abq.gzhubu.top

echo $((1 + 2 * 3))
来源：http://rfg.ydzc1.top

[R28] 浮点运算
来源：http://dzi.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://czv.hesvh.cn

[R29] 定义函数
来源：http://vnx.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://unt.daria6918.cn

[R30] 函数返回状态码
来源：http://zdz.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://ohn.9152youxi.cn

[R31] 局部变量
来源：http://pam.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://pmg.fzhhl.top

[R32] 参数个数校验
来源：http://hcy.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zxz.cheryme.top

[R33] 捕获错误并提示行号
来源：http://lxv.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kgy.redwolf501.top

[R34] 退出时清理
来源：http://mbb.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://nnh.yueranfly.top

[R35] 后台执行并等待
来源：http://hbr.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ihl.hesvh.cn

[R36] 并发执行多个任务
来源：http://uuw.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dhx.zhengqikj.top

[R37] 把输出赋给变量
来源：http://ksz.xinyue.icu

files=$(ls -1)
来源：http://umw.aibaodan.cn

[R38] 管道串联
来源：http://ezf.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://jct.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://zdt.hywenlv.cn

cmd > out.log 2>&1
来源：http://gbt.gotoacloud.top

[R40] 追加写日志
来源：http://qzg.yuanzhike.top

echo "log" >> out.log
来源：http://rrq.tianlin.xyz

[R41] 丢弃输出
来源：http://idu.hcnkem.com

cmd >/dev/null 2>&1
来源：http://gjw.ydjk.org.cn

[R42] 输入重定向
来源：http://cvt.cqqwz.cn

wc -l < a.txt
来源：http://ejn.aibaodan.cn

[R43] 按名字查找文件
来源：http://ssf.hfpthk.cn

find . -name "*.log" -type f
来源：http://vfs.hywenlv.cn

[R44] 按修改时间查找
来源：http://gvw.9152youxi.cn

find . -mtime -7 -type f
来源：http://wyg.cheryme.top

[R45] 批量删除
来源：http://ahb.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://heg.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://zef.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rza.redwolf501.top

[R47] sed 单行替换
来源：http://vkm.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://kwj.chenzaomai.com

[R48] awk 取指定列
来源：http://xby.fehbvm.com

awk '{print $1, $3}' a.txt
来源：http://kyn.bjfxy.top

[R49] awk 带条件
来源：http://ldr.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sjr.fzhhl.top

[R50] awk 求和
来源：http://mqn.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yhy.guannengcc.top

[R51] 排序去重取前几
来源：http://plc.yangfankeji.com

sort a.txt | uniq -c | sort -rn | head
来源：http://yui.vqdsnc.cn

[R52] 统计行数
来源：http://cof.ehwqpu.com

wc -l a.txt
来源：http://cwf.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://sjv.pycfn.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kgs.aizwys.cn

[R54] 比较两个文件
来源：http://fox.zhaomingkeji.xyz

diff a.txt b.txt
来源：http://ngf.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://xuv.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jqn.yueranfly.top

[R56] 远程拷贝
来源：http://hjz.dashuyun.cn

scp file user@host:/path/
来源：http://dop.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://pri.andypj.xyz

ssh user@host 'uptime'
来源：http://cuu.chenjidiqi.icu

[R58] 下载文件
来源：http://mvx.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vgb.chenlongwang.top

[R59] 发 POST JSON
来源：http://fgf.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iqh.jlsjyb.cn

[R60] 只看 HTTP 状态码
来源：http://klh.quarkkingdee.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pwn.xziqi.cn

[R61] 磁盘占用
来源：http://qvo.ydjk.org.cn

df -h;  du -sh *
来源：http://txl.yonumen.top

[R62] 找最占空间的文件
来源：http://vbc.tanke756.top

du -ah . | sort -rh | head -10
来源：http://plp.jlsjyb.cn

[R63] 内存与进程
来源：http://qmm.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://fuq.jinyuanbaomall.cn

[R64] 结束进程
来源：http://jmd.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://tqg.zycfv.cn

[R65] 查看端口占用
来源：http://mif.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qtx.jinqigufen.top

[R66] 定时任务
来源：http://xmy.zhixingplan.top

crontab -e;  crontab -l
来源：http://wht.yj20258888.top

[R67] 生成随机十六进制串
来源：http://glx.dashuyun.cn

openssl rand -hex 16
来源：http://yyg.jiagoushi.top

[R68] 计算文件校验值
来源：http://xjw.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zgk.meibo888.top

[R69] 生成随机密码
来源：http://cew.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://zpr.yj20258.top

[R70] 时间戳与互转
来源：http://hhx.smart0.xyz

date +%s;  date -d @1700000000
来源：http://klz.daria6918.cn

[R71] 日期格式化
来源：http://ucl.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://fzz.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://svc.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xtr.tian-w.cn

[R73] 分割大日志
来源：http://elr.ehwqpu.com

split -l 1000 big.log part_
来源：http://ppv.52xcode.cn

[R74] 批量重命名
来源：http://hdh.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bir.guannengcc.top

[R75] 导出环境变量
来源：http://pkw.tian-w.cn


<!-- 参考信息 -->