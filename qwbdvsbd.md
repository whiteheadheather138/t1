代发 wailian999

SELECT * FROM users;
来源：http://rka.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://jhk.hcnkem.com

SELECT id, name FROM users;
来源：http://omi.jqgufenzy.top

[Q17] 条件查询
来源：http://oal.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://igf.shanyushiyangtech.top

[Q18] 模糊匹配
来源：http://rps.tarul.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mxw.9152youxi.cn

[Q19] 范围查询
来源：http://qmj.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pte.chenlongwang.top

[Q20] IN 列表
来源：http://srz.fzhhl.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://skd.jiagoushi.top

[Q21] 空值判断
来源：http://agj.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mze.zhengqikj.top

[Q22] 排序
来源：http://gjh.shzxlz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://frh.shuidangran.top

[Q23] 分页
来源：http://tdj.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xhh.fanxiaobao.xyz

[Q24] 去重
来源：http://kwa.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://jti.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://gfo.gaohongyu789.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pxs.redwolf501.top

[Q26] 计数
来源：http://sut.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://gqw.gaohongyu789.top

[Q27] 条件计数
来源：http://vxv.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xgi.yj202588.top

[Q28] 求和与平均
来源：http://ekp.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mmv.316326.xyz

[Q29] 最大最小值
来源：http://sgn.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gfh.feifeiyinyue.top

[Q30] 分组统计
来源：http://ypv.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gdt.jianghu66.top

[Q31] 分组后过滤
来源：http://qpm.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xam.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://xyx.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kag.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yge.gzhubu.top

[Q33] 多列分组
来源：http://olg.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xhk.yuxming.cn

[Q34] 每组取第一条
来源：http://ujw.jyoumei.cn

SELECT * FROM (
来源：http://lda.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tzy.chenzaomai.com

) t WHERE rn = 1;
来源：http://wsn.fanxiaobao.xyz

[Q35] 内连接
来源：http://fwg.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yqn.yuanzhike.top

[Q36] 左连接
来源：http://tli.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wog.cucudq.cn

[Q37] 右连接
来源：http://tdg.guowangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nww.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://clo.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vcf.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://xll.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nft.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cvw.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fzn.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nsj.yj202588.top

[Q41] 多表连接
来源：http://dzl.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hyh.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://irl.zdbjq.cn

JOIN products p ON p.id = o.product_id;
来源：http://rnv.tanke756.top

[Q42] 连接条件附加过滤
来源：http://fzp.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://tyh.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rih.52xcode.cn

[Q43] 标量子查询
来源：http://ssz.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tzt.aibaodan.cn

[Q44] IN 子查询
来源：http://nmw.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://shv.pycfn.com

[Q45] EXISTS 判断存在
来源：http://mvv.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://szf.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://tmv.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wyr.aizwys.cn

[Q47] 与平均值比较
来源：http://xge.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ypv.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://emw.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://avy.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://sgh.zdqjudy.top

[Q49] 更新单行
来源：http://xgt.daria6918.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vzd.fanxiaobao.xyz

[Q50] 批量更新
来源：http://fkd.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ica.jqgfzy.top

[Q51] 用子查询更新
来源：http://cqx.yongpay.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vbz.gzhubu.top

[Q52] 删除指定行
来源：http://vtg.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://hhf.shzxlz.cn

[Q53] 按条件删除
来源：http://cft.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ihd.jiagoushi.top

[Q54] 清空表
来源：http://gbp.chenzaomai.com

TRUNCATE TABLE logs;
来源：http://rxn.hcnkem.com

[Q55] 排名（并列占位）
来源：http://xdq.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fvd.zhixingplan.top

[Q56] 密集排名（并列不占位）
来源：http://pyp.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wsq.hfpthk.cn

[Q57] 行号
来源：http://xhr.uphjek.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xxz.vehdjk.com

[Q58] 累计求和
来源：http://nia.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bbh.daxiang520.top

[Q59] 分组内累计
来源：http://wdx.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tlh.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://yrn.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pyi.quarkkingdee.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mdq.nanxinkj.top

[Q61] 移动平均
来源：http://yxu.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wbt.yj20258.top

[Q62] 分组占比
来源：http://qsw.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hby.yanxiufei.cn

[Q63] 开启事务
来源：http://zko.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://cwg.xziqi.cn

[Q64] 提交事务
来源：http://dff.zhiwuduotai.top

COMMIT;
来源：http://tym.epnwcf.com

[Q65] 回滚事务
来源：http://oro.aizwys.cn

ROLLBACK;
来源：http://gqt.pengpengdd.cyou

[Q66] 行锁查询
来源：http://gih.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sso.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://fub.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://flo.tanke756.top

[Q68] 保存点
来源：http://lxh.zdbjq.cn

SAVEPOINT sp1;
来源：http://alx.mhx1999.top

ROLLBACK TO sp1;
来源：http://rhh.hnxiangtu.top

[Q69] 查看执行计划
来源：http://mqw.hcnkem.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dvt.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://rqm.fehbvm.com

ANALYZE TABLE users;
来源：http://djq.fktsv.cn

[Q71] 查看建表语句
来源：http://bbn.fanxiaobao.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rpk.aibaodan.cn

[Q72] 查看索引
来源：http://vtw.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://dgg.yonumen.top

[Q73] 查看表状态
来源：http://nzi.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://oyo.zhoulong.xyz

[Q74] 强制使用索引
来源：http://yzg.sufxvd.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zli.cdnleiting.top

[Q75] 日期格式化
来源：http://zka.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tdo.bjfxy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vzy.redwolf501.top

[Q76] 按天统计
来源：http://ysh.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xmn.jianghu66.top

[Q77] 时间加减
来源：http://pwk.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pyl.shangyingyoupin.top

[Q78] 当前时间
来源：http://kzs.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://imw.fengsongda.top

[Q79] 字符串拼接
来源：http://gik.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fow.yuxming.cn

[Q80] 字符串截取
来源：http://nuo.xinyue.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://anh.cheryme.top

[Q81] 字符串替换
来源：http://qyx.c1oappe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ert.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://sbu.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xyd.ydjk.org.cn

[Q83] 大小写转换
来源：http://vfn.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://enu.haohaochexian.top

[Q84] 去除首尾空格
来源：http://hon.jlsjyb.cn

SELECT TRIM(name) FROM users;
来源：http://leg.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://seg.cdnleiting.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ral.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://pfi.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oym.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://qva.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mwl.jinqigufen.top

[Q88] 行转列（条件聚合）
来源：http://pxx.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://msr.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://emy.nwbrower.top

[Q89] 判断表是否存在
来源：http://aab.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rgi.daria6918.cn

[Q90] 生成序号列
来源：http://kzg.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://saw.sweek.top

================================================================================
来源：http://abd.nwbrower.top

R. Bash 专题
来源：http://grk.sysykeji.top

================================================================================
来源：http://cqd.xylfe.cn

[R01] shebang 与严格模式
来源：http://xlr.c1oappe.top

#!/usr/bin/env bash
来源：http://ogl.jinghuilouyu.cn

set -euo pipefail
来源：http://msi.cdnleiting.top

[R02] 变量赋值与使用
来源：http://azw.xylfe.cn

name="Tom"; echo "$name"
来源：http://fjj.wangdashe.top

[R03] 只读变量
来源：http://dhp.ehwqpu.com

readonly PI=3.14
来源：http://itr.cashguo.top

[R04] 位置参数
来源：http://vvr.zhiwuduotai.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://irx.guannengcc.top

[R05] 参数默认值
来源：http://ufz.meibo888.top

name="${1:-default}"
来源：http://daq.epnwcf.com

[R06] 判断命令是否存在
来源：http://kro.zhengqikj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aol.hywenlv.cn

[R07] if 判断文件
来源：http://uvv.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ioa.yanxiufei.cn

[R08] 数值比较
来源：http://vgu.fzhhl.top

if (( a > b )); then echo "a 更大"; fi
来源：http://smr.hongshengwenyu.top

[R09] 字符串比较
来源：http://axt.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cnb.smart0.xyz

[R10] 正则匹配
来源：http://nzy.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://shn.shzxlz.cn

[R11] case 多分支
来源：http://roo.zdbjq.cn

case "$1" in
来源：http://wom.gaohongyu789.top

start) echo "启动" ;;
来源：http://rwf.xuanzx.com

stop)  echo "停止" ;;
来源：http://swh.cucudq.cn

*)     echo "未知命令" ;;
来源：http://tiq.tanke756.top

esac
来源：http://drf.shuidangran.top

[R12] for 遍历文件
来源：http://tto.fengsongda.top

for f in *.txt; do echo "$f"; done
来源：http://zha.yuanzhike.top

[R13] for 计数循环
来源：http://xff.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://vdq.svipenyu.cn

[R14] C 风格 for
来源：http://nqr.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nfs.jinyuanbaomall.cn

[R15] while 逐行读文件
来源：http://mzt.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://drr.aizwys.cn

[R16] until 等待条件
来源：http://ilf.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tlr.sweek.top

[R17] 数组定义与取值
来源：http://auo.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://ede.jlsjyb.cn

[R18] 遍历数组
来源：http://rsq.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://djb.jiagoushi.top

[R19] 数组长度
来源：http://mdm.guannengcc.top

echo "${#arr[@]}"
来源：http://aaj.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://spp.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gdi.hongshengwenyu.top

[R21] 字符串长度
来源：http://msi.fzhhl.top

echo "${#s}"
来源：http://ztz.hcnkem.com

[R22] 截取子串
来源：http://hvt.havefunace.top

echo "${s:0:5}"
来源：http://xwz.fzhhl.top

[R23] 字符串替换
来源：http://gpl.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vrl.nwbrower.top

[R24] 大小写转换
来源：http://uam.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://bij.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://air.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lvv.bjfxy.top

[R26] 命令替换
来源：http://hfb.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://akw.jiagoushi.top

[R27] 算术展开
来源：http://gyl.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://kyh.9152youxi.cn

[R28] 浮点运算
来源：http://zft.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://hcn.iojbl.cn

[R29] 定义函数
来源：http://mmu.fengsongda.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dky.sjlbkw.cn

[R30] 函数返回状态码
来源：http://yqu.yanxiufei.cn

f() { return 0; }; f || echo "失败了"
来源：http://ugi.52xcode.cn

[R31] 局部变量
来源：http://iue.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://vqh.jinqigufen.top

[R32] 参数个数校验
来源：http://uhs.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ang.bjfxy.top

[R33] 捕获错误并提示行号
来源：http://fqw.hcnkem.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nha.316326.xyz

[R34] 退出时清理
来源：http://hqu.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://oxj.daria6918.cn

[R35] 后台执行并等待
来源：http://gkp.snrcjt.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vol.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://rhd.hywenlv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lpk.ybcxt.top

[R37] 把输出赋给变量
来源：http://hkh.jinqigfzy.top

files=$(ls -1)
来源：http://qod.jqgfzy.top

[R38] 管道串联
来源：http://qos.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://ytl.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://xlc.sweek.top

cmd > out.log 2>&1
来源：http://jck.pengpengdd.cyou

[R40] 追加写日志
来源：http://tes.ydjk.org.cn

echo "log" >> out.log
来源：http://lhi.fehbvm.com

[R41] 丢弃输出
来源：http://zdd.snrcjt.cn

cmd >/dev/null 2>&1
来源：http://ypg.dianchejie.cn

[R42] 输入重定向
来源：http://pww.wangshuangyany.cn

wc -l < a.txt
来源：http://fry.yonumen.top

[R43] 按名字查找文件
来源：http://wrq.aibaodan.cn

find . -name "*.log" -type f
来源：http://onk.ybcxt.top

[R44] 按修改时间查找
来源：http://gzg.chenzaomai.com

find . -mtime -7 -type f
来源：http://yao.zhijiandao.cn

[R45] 批量删除
来源：http://bcu.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://bpb.tianlin.xyz

[R46] 递归替换文件内容
来源：http://jhp.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ajt.yfazqb.com

[R47] sed 单行替换
来源：http://cdn.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dak.c1oappe.top

[R48] awk 取指定列
来源：http://nmm.cqqwz.cn

awk '{print $1, $3}' a.txt
来源：http://rca.vqdsnc.cn

[R49] awk 带条件
来源：http://ctb.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wre.ydzc1.top

[R50] awk 求和
来源：http://nll.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://jkp.zycfv.cn

[R51] 排序去重取前几
来源：http://aju.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://axa.iojbl.cn

[R52] 统计行数
来源：http://cer.jinghuilouyu.cn

wc -l a.txt
来源：http://wqo.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://tsw.vehdjk.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bdf.bjfxy.top

[R54] 比较两个文件
来源：http://jfz.wangdashe.top

diff a.txt b.txt
来源：http://sql.uphjek.com

[R55] 压缩与解压
来源：http://mkt.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wdi.gzhubu.top

[R56] 远程拷贝
来源：http://nnv.shanyushiyangtech.top

scp file user@host:/path/
来源：http://fvp.sufxvd.cn

[R57] 远程执行命令
来源：http://bch.jyoumei.cn

ssh user@host 'uptime'
来源：http://avj.gogol.net.cn

[R58] 下载文件
来源：http://wuf.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://amw.jqgfzy.top

[R59] 发 POST JSON
来源：http://uoq.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://axx.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://jqi.zhiwuduotai.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://twv.tian-w.cn

[R61] 磁盘占用
来源：http://yru.nanxinkj.top

df -h;  du -sh *
来源：http://dvk.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://uzo.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://cfm.yuanzhike.top

[R63] 内存与进程
来源：http://gor.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://pab.tianlin.xyz

[R64] 结束进程
来源：http://ymk.smart0.xyz

kill -9 $(pgrep -f app.py)
来源：http://fib.yj20258888.top

[R65] 查看端口占用
来源：http://fhc.jinghuilouyu.cn


<!-- 参考信息 -->