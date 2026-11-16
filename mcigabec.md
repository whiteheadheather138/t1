代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://ixy.shangyingyoupin.top

[Q22] 排序
来源：http://cei.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lkg.jiagoushi.top

[Q23] 分页
来源：http://mnv.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zhb.epnwcf.com

[Q24] 去重
来源：http://xid.daria6918.cn

SELECT DISTINCT city FROM users;
来源：http://zdd.yonumen.top

[Q25] 只取前 N 条
来源：http://hmo.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hig.yj20258888.top

[Q26] 计数
来源：http://npx.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://uvx.yj202588.top

[Q27] 条件计数
来源：http://udk.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://duc.nanxinkj.top

[Q28] 求和与平均
来源：http://liu.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hjt.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://kpt.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://anb.vqdsnc.cn

[Q30] 分组统计
来源：http://img.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dev.hammf.cn

[Q31] 分组后过滤
来源：http://pzx.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://axm.sxryk.cn

[Q32] 分组拼接字符串
来源：http://rzp.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kca.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ija.xylfe.cn

[Q33] 多列分组
来源：http://jkx.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://myj.hesvh.cn

[Q34] 每组取第一条
来源：http://pev.cdnleiting.top

SELECT * FROM (
来源：http://mpk.zhengqikj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bbd.hongshengwenyu.top

) t WHERE rn = 1;
来源：http://cvi.0kj1m.cn

[Q35] 内连接
来源：http://pus.316326.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://axr.316326.xyz

[Q36] 左连接
来源：http://ynr.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://anp.316326.xyz

[Q37] 右连接
来源：http://ogq.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jrg.gzhubu.top

[Q38] 全外连接（PostgreSQL）
来源：http://xkz.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tse.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://ucs.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qbz.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lqq.nanxuanxn.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ggj.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xyb.wangshuangyany.cn

[Q41] 多表连接
来源：http://lwg.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tpk.svipenyu.cn

JOIN users u ON u.id = o.user_id
来源：http://tda.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://zuu.tarul.cn

[Q42] 连接条件附加过滤
来源：http://aea.xylfe.cn

SELECT u.name, o.amount FROM users u
来源：http://vpw.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://log.zycfv.cn

[Q43] 标量子查询
来源：http://tmd.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://itm.pengpengdd.cyou

[Q44] IN 子查询
来源：http://ehf.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dpc.yongpay.top

[Q45] EXISTS 判断存在
来源：http://qmg.smart0.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zme.yvedp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yvm.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://onz.sufxvd.cn

[Q47] 与平均值比较
来源：http://knc.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://spv.fktsv.cn

[Q48] CTE 公用表表达式
来源：http://agy.jinyuanbaomall.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pcc.sufxvd.cn

SELECT * FROM t WHERE c > 5;
来源：http://moq.chenzaomai.com

[Q49] 更新单行
来源：http://gjw.ywan-chungtsiang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wim.aizwys.cn

[Q50] 批量更新
来源：http://esv.hnqzz.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uoe.daria6918.cn

[Q51] 用子查询更新
来源：http://vgp.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qzt.ehwqpu.com

[Q52] 删除指定行
来源：http://icz.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://owg.pengpengdd.cyou

[Q53] 按条件删除
来源：http://ciu.tianlin.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hsi.feifeiyinyue.top

[Q54] 清空表
来源：http://hex.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://qsx.yuxming.cn

[Q55] 排名（并列占位）
来源：http://qyi.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dzo.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://vke.fengsongda.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uym.yvedp.cn

[Q57] 行号
来源：http://ohq.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://icd.yanxiufei.cn

[Q58] 累计求和
来源：http://pmf.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fwz.xylfe.cn

[Q59] 分组内累计
来源：http://nhr.hcnkem.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wiq.yj202588.top

[Q60] 取上一行 / 下一行
来源：http://vva.sufxvd.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nkb.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eip.xuanzx.com

[Q61] 移动平均
来源：http://lkx.jqgufenzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mqr.yongpay.top

[Q62] 分组占比
来源：http://tfn.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://edj.hnqzz.top

[Q63] 开启事务
来源：http://nsh.pycfn.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ypw.52xcode.cn

[Q64] 提交事务
来源：http://mcy.hongshengwenyu.top

COMMIT;
来源：http://kyl.nanxinkj.top

[Q65] 回滚事务
来源：http://jjg.jlsjyb.cn

ROLLBACK;
来源：http://gwc.ydjk.org.cn

[Q66] 行锁查询
来源：http://gdu.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rdw.birdmap.top

[Q67] 设置隔离级别
来源：http://unc.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mfm.xinyue.icu

[Q68] 保存点
来源：http://fwu.sjlbkw.cn

SAVEPOINT sp1;
来源：http://nac.guowangkeji.top

ROLLBACK TO sp1;
来源：http://xim.ydzc1.top

[Q69] 查看执行计划
来源：http://hrv.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zzh.guannengcc.top

[Q70] 更新统计信息
来源：http://ijh.vqdsnc.cn

ANALYZE TABLE users;
来源：http://pok.hnxiangtu.top

[Q71] 查看建表语句
来源：http://cju.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://auz.zhengqikj.top

[Q72] 查看索引
来源：http://fss.cheryme.top

SHOW INDEX FROM users;
来源：http://qdt.aizwys.cn

[Q73] 查看表状态
来源：http://ely.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ukw.ctjpmb.com

[Q74] 强制使用索引
来源：http://vlg.fehbvm.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sqk.daxiang520.top

[Q75] 日期格式化
来源：http://apo.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vbg.hcnkem.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ntq.yonumen.top

[Q76] 按天统计
来源：http://qhh.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tfx.ivvv.top

[Q77] 时间加减
来源：http://nij.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fqm.yvedp.cn

[Q78] 当前时间
来源：http://nil.hfpthk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sas.epnwcf.com

[Q79] 字符串拼接
来源：http://opm.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zdu.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://eza.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://egi.guowangkeji.top

[Q81] 字符串替换
来源：http://wlg.tarul.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zfl.jqgufenzy.top

[Q82] 字符长度与字节长度
来源：http://hlk.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tbu.hesvh.cn

[Q83] 大小写转换
来源：http://ghp.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fsl.snrcjt.cn

[Q84] 去除首尾空格
来源：http://ets.gogol.net.cn

SELECT TRIM(name) FROM users;
来源：http://rlu.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://nay.ehwqpu.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://stl.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://gbc.yj202588.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pmz.xinyue.icu

[Q87] JSON 字段做条件
来源：http://bpr.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cfx.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://faj.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wya.ivvv.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://knh.52xcode.cn

[Q89] 判断表是否存在
来源：http://ipj.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lxb.zdbjq.cn

[Q90] 生成序号列
来源：http://mfa.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hki.snrcjt.cn

================================================================================
来源：http://xri.chenjidiqi.icu

R. Bash 专题
来源：http://nwl.shzxlz.cn

================================================================================
来源：http://ssy.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://rwo.sysykeji.top

#!/usr/bin/env bash
来源：http://okd.52xcode.cn

set -euo pipefail
来源：http://nnu.tanke756.top

[R02] 变量赋值与使用
来源：http://wxe.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://ftm.mhx1999.top

[R03] 只读变量
来源：http://yja.smart0.xyz

readonly PI=3.14
来源：http://lzi.shanyushiyangtech.top

[R04] 位置参数
来源：http://xrn.chenzaomai.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cxh.hnxiangtu.top

[R05] 参数默认值
来源：http://pyi.pycfn.com

name="${1:-default}"
来源：http://iwu.hfpthk.cn

[R06] 判断命令是否存在
来源：http://ppi.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ksu.9152youxi.cn

[R07] if 判断文件
来源：http://kat.zdqjudy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gas.feifeiyinyue.top

[R08] 数值比较
来源：http://djb.jiagoushi.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nxv.zhoulong.xyz

[R09] 字符串比较
来源：http://bls.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ura.zhongyouzk.top

[R10] 正则匹配
来源：http://jid.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xby.cqqwz.cn

[R11] case 多分支
来源：http://lqz.zhijiandao.cn

case "$1" in
来源：http://yle.fktsv.cn

start) echo "启动" ;;
来源：http://wkx.jianghu66.top

stop)  echo "停止" ;;
来源：http://nml.fktsv.cn

*)     echo "未知命令" ;;
来源：http://avk.fengsongda.top

esac
来源：http://vyc.0kj1m.cn

[R12] for 遍历文件
来源：http://upj.jinqigufen.top

for f in *.txt; do echo "$f"; done
来源：http://kxs.0kj1m.cn

[R13] for 计数循环
来源：http://wrm.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://rqh.hongshengwenyu.top

[R14] C 风格 for
来源：http://dpc.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nef.yangfankeji.com

[R15] while 逐行读文件
来源：http://vqa.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hub.c1oappe.top

[R16] until 等待条件
来源：http://ocr.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zrf.pengpengdd.cyou

[R17] 数组定义与取值
来源：http://akk.chenlongwang.top

arr=(a b c); echo "${arr[0]}"
来源：http://kin.yvedp.cn

[R18] 遍历数组
来源：http://bwm.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sgx.hesvh.cn

[R19] 数组长度
来源：http://lvx.gogol.net.cn

echo "${#arr[@]}"
来源：http://jbr.ctjpmb.com

[R20] 关联数组（字典）
来源：http://kxb.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ems.aizwys.cn

[R21] 字符串长度
来源：http://kod.9152youxi.cn

echo "${#s}"
来源：http://zub.havefunace.top

[R22] 截取子串
来源：http://mjs.cashguo.top

echo "${s:0:5}"
来源：http://bvw.yangfankeji.com

[R23] 字符串替换
来源：http://nwv.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ntg.hysaishi.cn

[R24] 大小写转换
来源：http://kro.zhixingplan.top

echo "${s^^}"; echo "${s,,}"
来源：http://ozi.kuanghao11.cn

[R25] 去后缀 / 去前缀
来源：http://ach.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qmk.tarul.cn

[R26] 命令替换
来源：http://num.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://mwz.ivvv.top

[R27] 算术展开
来源：http://ymp.ydzc1.top

echo $((1 + 2 * 3))
来源：http://gqk.hnqzz.top

[R28] 浮点运算
来源：http://izo.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://jla.zdqjudy.top

[R29] 定义函数
来源：http://dbw.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lek.shzxlz.cn

[R30] 函数返回状态码
来源：http://bku.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://tfg.nanxuanxn.top

[R31] 局部变量
来源：http://kyv.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://elo.gzhubu.top

[R32] 参数个数校验
来源：http://exs.cucudq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nvb.sweek.top

[R33] 捕获错误并提示行号
来源：http://prq.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qww.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://xai.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://plx.ctjpmb.com

[R35] 后台执行并等待
来源：http://gxh.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rjt.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://xre.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://okj.yj20258.top

[R37] 把输出赋给变量
来源：http://ahj.ctjpmb.com

files=$(ls -1)
来源：http://ggi.ywan-chungtsiang.top

[R38] 管道串联
来源：http://lgl.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://ets.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://qmi.zhixingplan.top

cmd > out.log 2>&1
来源：http://cco.zhongyouzk.top

[R40] 追加写日志
来源：http://wpg.aibaodan.cn

echo "log" >> out.log
来源：http://kxp.zhongyouzk.top

[R41] 丢弃输出
来源：http://rcg.aibaodan.cn

cmd >/dev/null 2>&1
来源：http://bqb.ppjwa.cn

[R42] 输入重定向
来源：http://vxp.yuanzhike.top

wc -l < a.txt
来源：http://aoy.jqgfzy.top

[R43] 按名字查找文件
来源：http://eym.shuidangran.top

find . -name "*.log" -type f
来源：http://qml.yfazqb.com

[R44] 按修改时间查找
来源：http://gew.zhoulong.xyz

find . -mtime -7 -type f
来源：http://jza.aibaodan.cn

[R45] 批量删除
来源：http://nxv.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://zoq.cucudq.cn

[R46] 递归替换文件内容
来源：http://ock.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lvh.feifeiyinyue.top

[R47] sed 单行替换
来源：http://nto.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://zcb.aizwys.cn

[R48] awk 取指定列
来源：http://ceq.ydzc1.top

awk '{print $1, $3}' a.txt
来源：http://fuv.jinqigfzy.top

[R49] awk 带条件
来源：http://dup.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gdj.dianchejie.cn

[R50] awk 求和
来源：http://sfa.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://fmb.hcnkem.com

[R51] 排序去重取前几
来源：http://xsa.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ywi.daxiang520.top

[R52] 统计行数
来源：http://fel.gogol.net.cn

wc -l a.txt
来源：http://sxi.tanke756.top

[R53] 查看文件头与实时尾
来源：http://ctc.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rwt.xziqi.cn

[R54] 比较两个文件
来源：http://dug.316326.xyz

diff a.txt b.txt
来源：http://tds.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://sho.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kup.ivvv.top

[R56] 远程拷贝
来源：http://hzm.guannengcc.top

scp file user@host:/path/
来源：http://lux.yueranfly.top

[R57] 远程执行命令
来源：http://opn.pycfn.com

ssh user@host 'uptime'
来源：http://oek.haohaochexian.top

[R58] 下载文件
来源：http://mgd.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ihu.mhx1999.top

[R59] 发 POST JSON
来源：http://lfr.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fin.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://hmt.yongpay.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gvo.316326.xyz

[R61] 磁盘占用
来源：http://bsn.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://hem.cheryme.top

[R62] 找最占空间的文件
来源：http://umu.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://saz.vqdsnc.cn

[R63] 内存与进程
来源：http://zsf.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://siw.0kj1m.cn

[R64] 结束进程
来源：http://fln.daxiang520.top

kill -9 $(pgrep -f app.py)
来源：http://agl.aibaodan.cn

[R65] 查看端口占用
来源：http://qfd.zdbjq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mlp.gotoacloud.top

[R66] 定时任务
来源：http://rnx.yvedp.cn

crontab -e;  crontab -l
来源：http://lbb.sjlbkw.cn

[R67] 生成随机十六进制串
来源：http://sbn.chenzaomai.com

openssl rand -hex 16
来源：http://aki.yuanzhike.top

[R68] 计算文件校验值
来源：http://cov.hammf.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rvt.chenjidiqi.icu

[R69] 生成随机密码
来源：http://oeo.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://hke.hammf.cn

[R70] 时间戳与互转
来源：http://iar.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://ywd.yj202588.top

[R71] 日期格式化
来源：http://fdj.jyoumei.cn


<!-- 参考信息 -->