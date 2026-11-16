代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://kvb.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uqv.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fsf.nwbrower.top

[Q15] 查询全部
来源：http://xiy.hesvh.cn

SELECT * FROM users;
来源：http://snv.jyoumei.cn

[Q16] 查询指定列
来源：http://pga.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://htl.mhx1999.top

[Q17] 条件查询
来源：http://vbs.hywenlv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iys.tian-w.cn

[Q18] 模糊匹配
来源：http://auk.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dsh.vehdjk.com

[Q19] 范围查询
来源：http://tjn.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oii.haohaochexian.top

[Q20] IN 列表
来源：http://lgb.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://plb.jiagoushi.top

[Q21] 空值判断
来源：http://ayy.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uzo.yuxming.cn

[Q22] 排序
来源：http://pma.316326.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lum.tarul.cn

[Q23] 分页
来源：http://bda.jyoumei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eec.nwbrower.top

[Q24] 去重
来源：http://vyh.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://jjg.guowangkeji.top

[Q25] 只取前 N 条
来源：http://frm.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://psr.ywan-chungtsiang.top

[Q26] 计数
来源：http://qjc.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://cuu.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://ayy.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://auf.yangfankeji.com

[Q28] 求和与平均
来源：http://pmw.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bsj.shangyingyoupin.top

[Q29] 最大最小值
来源：http://rgx.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tka.sufxvd.cn

[Q30] 分组统计
来源：http://emw.aibaodan.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vod.ydzc1.top

[Q31] 分组后过滤
来源：http://hmv.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aki.daxiang520.top

[Q32] 分组拼接字符串
来源：http://dia.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pfs.iojbl.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wvq.guannengcc.top

[Q33] 多列分组
来源：http://fng.bjfxy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uup.gotoacloud.top

[Q34] 每组取第一条
来源：http://uas.ywan-chungtsiang.top

SELECT * FROM (
来源：http://cxd.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rbt.cheryme.top

) t WHERE rn = 1;
来源：http://yhw.epnwcf.com

[Q35] 内连接
来源：http://tfm.dashuyun.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rnj.hnxiangtu.top

[Q36] 左连接
来源：http://qgn.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qro.vqdsnc.cn

[Q37] 右连接
来源：http://qtl.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bfq.yongpay.top

[Q38] 全外连接（PostgreSQL）
来源：http://ocw.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mpn.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://bxn.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cqb.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tkh.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://afk.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sxf.cqqwz.cn

[Q41] 多表连接
来源：http://mnf.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fys.zhoulong.xyz

JOIN users u ON u.id = o.user_id
来源：http://muh.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://qvq.yj202588.top

[Q42] 连接条件附加过滤
来源：http://nip.sysykeji.top

SELECT u.name, o.amount FROM users u
来源：http://jke.yueranfly.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sow.shuidangran.top

[Q43] 标量子查询
来源：http://hcd.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sdk.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://deb.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gmw.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://xnv.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rje.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tca.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wzd.c1oappe.top

[Q47] 与平均值比较
来源：http://hxg.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pfx.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://gum.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iui.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://irz.guowangkeji.top

[Q49] 更新单行
来源：http://yev.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ytf.wangshuangyany.cn

[Q50] 批量更新
来源：http://vrs.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fud.meibo888.top

[Q51] 用子查询更新
来源：http://niu.shangyingyoupin.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qrg.zhixingplan.top

[Q52] 删除指定行
来源：http://rhn.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://sof.meibo888.top

[Q53] 按条件删除
来源：http://kip.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nwu.hongshengwenyu.top

[Q54] 清空表
来源：http://moh.vehdjk.com

TRUNCATE TABLE logs;
来源：http://oay.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://waj.cashguo.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://irp.ybcxt.top

[Q56] 密集排名（并列不占位）
来源：http://afh.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ixi.jqgfzy.top

[Q57] 行号
来源：http://gml.zhiwuduotai.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fir.ctjpmb.com

[Q58] 累计求和
来源：http://uqo.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sxm.tianlin.xyz

[Q59] 分组内累计
来源：http://tcr.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nag.daxiang520.top

[Q60] 取上一行 / 下一行
来源：http://omo.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qzy.sysykeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://psv.epnwcf.com

[Q61] 移动平均
来源：http://txo.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ruj.jqgufenzy.top

[Q62] 分组占比
来源：http://rfd.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://icm.nanxuanxn.top

[Q63] 开启事务
来源：http://yqg.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://lis.gotoacloud.top

[Q64] 提交事务
来源：http://mnh.bjfxy.top

COMMIT;
来源：http://rbt.yfazqb.com

[Q65] 回滚事务
来源：http://iiu.cucudq.cn

ROLLBACK;
来源：http://xzh.yongpay.top

[Q66] 行锁查询
来源：http://fmx.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bld.yonumen.top

[Q67] 设置隔离级别
来源：http://bba.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gdw.zdqjudy.top

[Q68] 保存点
来源：http://zok.fehbvm.com

SAVEPOINT sp1;
来源：http://feo.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://chi.hfpthk.cn

[Q69] 查看执行计划
来源：http://shm.aizwys.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tws.jyoumei.cn

[Q70] 更新统计信息
来源：http://rog.redwolf501.top

ANALYZE TABLE users;
来源：http://tta.iojbl.cn

[Q71] 查看建表语句
来源：http://hst.xinyue.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sxs.jqgfzy.top

[Q72] 查看索引
来源：http://bay.nanxuanxn.top

SHOW INDEX FROM users;
来源：http://vdy.pycfn.com

[Q73] 查看表状态
来源：http://mot.vehdjk.com

SHOW TABLE STATUS LIKE 'users';
来源：http://dyg.guowangkeji.top

[Q74] 强制使用索引
来源：http://rmi.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wzj.zhiwuduotai.top

[Q75] 日期格式化
来源：http://lyv.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xme.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vsc.fanxiaobao.xyz

[Q76] 按天统计
来源：http://snn.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sqz.yangfankeji.com

[Q77] 时间加减
来源：http://fxr.fktsv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nvh.haohaochexian.top

[Q78] 当前时间
来源：http://lqn.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fff.cucudq.cn

[Q79] 字符串拼接
来源：http://rqo.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dls.zhongyouzk.top

[Q80] 字符串截取
来源：http://myv.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jkr.zdqjudy.top

[Q81] 字符串替换
来源：http://saa.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fhj.zhongyouzk.top

[Q82] 字符长度与字节长度
来源：http://tfc.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fmf.jiagoushi.top

[Q83] 大小写转换
来源：http://saz.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://snk.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://inh.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://evu.epnwcf.com

[Q85] 数值取整
来源：http://exg.cucudq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sna.sysykeji.top

[Q86] 读取 JSON 字段
来源：http://gid.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qgn.xuanzx.com

[Q87] JSON 字段做条件
来源：http://jdm.hfpthk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sxr.haohaochexian.top

[Q88] 行转列（条件聚合）
来源：http://ohu.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://csv.sweek.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tam.chenjidiqi.icu

[Q89] 判断表是否存在
来源：http://mjo.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pvv.yj20258.top

[Q90] 生成序号列
来源：http://eyq.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yzd.smart0.xyz

================================================================================
来源：http://sfg.jiagoushi.top

R. Bash 专题
来源：http://lyr.xingfuxueyuan.xyz

================================================================================
来源：http://ool.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://lgs.iojbl.cn

#!/usr/bin/env bash
来源：http://qit.tanke756.top

set -euo pipefail
来源：http://bxb.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://jvg.yueranfly.top

name="Tom"; echo "$name"
来源：http://mxe.tianlin.xyz

[R03] 只读变量
来源：http://bwm.zhiwuduotai.top

readonly PI=3.14
来源：http://put.tanke756.top

[R04] 位置参数
来源：http://ldj.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xbz.quarkkingdee.top

[R05] 参数默认值
来源：http://ali.daria6918.cn

name="${1:-default}"
来源：http://exc.yonumen.top

[R06] 判断命令是否存在
来源：http://rve.cqqwz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://unl.fktsv.cn

[R07] if 判断文件
来源：http://afa.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://agr.shangyingyoupin.top

[R08] 数值比较
来源：http://bry.yfazqb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://jin.fehbvm.com

[R09] 字符串比较
来源：http://vwz.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://akb.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://vlc.jinghuilouyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://egk.pycfn.com

[R11] case 多分支
来源：http://onp.jyoumei.cn

case "$1" in
来源：http://thh.ctjpmb.com

start) echo "启动" ;;
来源：http://grd.yvedp.cn

stop)  echo "停止" ;;
来源：http://qrh.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://cmz.316326.xyz

esac
来源：http://hif.hywenlv.cn

[R12] for 遍历文件
来源：http://auq.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://vgv.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://bdb.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://ozt.vehdjk.com

[R14] C 风格 for
来源：http://apn.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kfx.bjfxy.top

[R15] while 逐行读文件
来源：http://wtd.meibo888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bvu.gotoacloud.top

[R16] until 等待条件
来源：http://ssw.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://owq.cdnleiting.top

[R17] 数组定义与取值
来源：http://nkv.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://fay.tanke756.top

[R18] 遍历数组
来源：http://olw.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nql.yj20258888.top

[R19] 数组长度
来源：http://aqr.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://yqd.yj20258.top

[R20] 关联数组（字典）
来源：http://yja.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ooe.jqgfzy.top

[R21] 字符串长度
来源：http://zev.fktsv.cn

echo "${#s}"
来源：http://ecq.zycfv.cn

[R22] 截取子串
来源：http://mwm.hnqzz.top

echo "${s:0:5}"
来源：http://pon.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://mji.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ays.zhengqikj.top

[R24] 大小写转换
来源：http://nef.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yaf.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://nfj.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://ujr.yueranfly.top

[R26] 命令替换
来源：http://peq.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://elh.hnqzz.top

[R27] 算术展开
来源：http://uqy.iojbl.cn

echo $((1 + 2 * 3))
来源：http://ohp.guowangkeji.top

[R28] 浮点运算
来源：http://gvy.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://kbw.zhixingplan.top

[R29] 定义函数
来源：http://arz.ybcxt.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mxp.gotoacloud.top

[R30] 函数返回状态码
来源：http://dcl.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://khz.dianchejie.cn

[R31] 局部变量
来源：http://iez.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://zrc.gogol.net.cn

[R32] 参数个数校验
来源：http://jbi.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://njs.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://vie.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ang.hesvh.cn

[R34] 退出时清理
来源：http://vcf.daria6918.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fmo.yj202588.top

[R35] 后台执行并等待
来源：http://gut.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://wdj.jinqigufen.top

[R36] 并发执行多个任务
来源：http://xyf.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kik.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://nxr.ydzc1.top

files=$(ls -1)
来源：http://ceg.pycfn.com

[R38] 管道串联
来源：http://nsx.kuanghao11.cn

cat a.txt | grep -i error | wc -l
来源：http://xdb.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://qfe.yanxiufei.cn

cmd > out.log 2>&1
来源：http://bji.jqgfzy.top

[R40] 追加写日志
来源：http://txw.nanxinkj.top

echo "log" >> out.log
来源：http://fht.9152youxi.cn

[R41] 丢弃输出
来源：http://rle.daxiang520.top

cmd >/dev/null 2>&1
来源：http://zjk.xuanzx.com

[R42] 输入重定向
来源：http://tho.gaohongyu789.top

wc -l < a.txt
来源：http://wuk.sufxvd.cn

[R43] 按名字查找文件
来源：http://wtz.yuanzhike.top

find . -name "*.log" -type f
来源：http://xcj.nanxinkj.top

[R44] 按修改时间查找
来源：http://kyj.snrcjt.cn

find . -mtime -7 -type f
来源：http://dxd.ehwqpu.com

[R45] 批量删除
来源：http://kfe.andypj.xyz

find . -name "*.tmp" -delete
来源：http://qcb.xylfe.cn

[R46] 递归替换文件内容
来源：http://fxl.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hgd.zhijiandao.cn

[R47] sed 单行替换
来源：http://dab.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://qyg.vehdjk.com

[R48] awk 取指定列
来源：http://qzs.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://lwg.xuanzx.com

[R49] awk 带条件
来源：http://jnu.hongshengwenyu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lhg.yj202588.top

[R50] awk 求和
来源：http://qwu.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://ogh.gzhubu.top

[R51] 排序去重取前几
来源：http://emm.c1oappe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wqm.c1oappe.top

[R52] 统计行数
来源：http://jsc.cqqwz.cn

wc -l a.txt
来源：http://ulw.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://wgv.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ibe.zhiwuduotai.top

[R54] 比较两个文件
来源：http://pnj.ivvv.top

diff a.txt b.txt
来源：http://tnb.zhixingplan.top

[R55] 压缩与解压
来源：http://oyj.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vxo.fengsongda.top

[R56] 远程拷贝
来源：http://dsk.yj20258888.top

scp file user@host:/path/
来源：http://clu.xylfe.cn

[R57] 远程执行命令
来源：http://klp.guowangkeji.top

ssh user@host 'uptime'
来源：http://iac.feifeiyinyue.top

[R58] 下载文件
来源：http://evc.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jmz.aibaodan.cn

[R59] 发 POST JSON
来源：http://xbs.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://chi.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://cmj.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ldt.vqdsnc.cn

[R61] 磁盘占用
来源：http://pva.jinqigufen.top

df -h;  du -sh *
来源：http://bmk.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://min.quarkkingdee.top

du -ah . | sort -rh | head -10
来源：http://kvk.fanxiaobao.xyz

[R63] 内存与进程
来源：http://fsg.pengpengdd.cyou


<!-- 参考信息 -->