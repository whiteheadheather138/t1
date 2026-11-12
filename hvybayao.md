代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wnt.jyoumei.cn

[Q18] 模糊匹配
来源：http://sve.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xrp.zhixingplan.top

[Q19] 范围查询
来源：http://wui.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wxk.redwolf501.top

[Q20] IN 列表
来源：http://hfa.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tui.jqgufenzy.top

[Q21] 空值判断
来源：http://pte.xziqi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ggl.chenjidiqi.icu

[Q22] 排序
来源：http://ezy.jiagoushi.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mrg.hnxiangtu.top

[Q23] 分页
来源：http://fpv.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://osn.ctjpmb.com

[Q24] 去重
来源：http://rxw.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://yde.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://pzi.zdbjq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://chs.hywenlv.cn

[Q26] 计数
来源：http://wei.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://yeh.dianchejie.cn

[Q27] 条件计数
来源：http://bbd.zdbjq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://whf.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://mzs.cucudq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hyw.zycfv.cn

[Q29] 最大最小值
来源：http://gvn.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kxo.tanke756.top

[Q30] 分组统计
来源：http://irq.cqqwz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://msk.zhengqikj.top

[Q31] 分组后过滤
来源：http://zoj.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fkq.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://nog.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bdc.sjlbkw.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vdv.c1oappe.top

[Q33] 多列分组
来源：http://aoo.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pdw.yuanzhike.top

[Q34] 每组取第一条
来源：http://uab.zhiwuduotai.top

SELECT * FROM (
来源：http://qta.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wcj.zdbjq.cn

) t WHERE rn = 1;
来源：http://dfe.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://yho.uphjek.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sfa.meibo888.top

[Q36] 左连接
来源：http://ysx.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lwz.zhijiandao.cn

[Q37] 右连接
来源：http://tqm.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vth.jyoumei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gjg.yonumen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nkc.sxryk.cn

[Q39] 自连接（查上下级）
来源：http://efs.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bla.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://whv.kuanghao11.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lzy.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://teu.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://gmk.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uts.havefunace.top

JOIN users u ON u.id = o.user_id
来源：http://rko.52xcode.cn

JOIN products p ON p.id = o.product_id;
来源：http://lko.zhijiandao.cn

[Q42] 连接条件附加过滤
来源：http://hem.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://lib.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mej.hesvh.cn

[Q43] 标量子查询
来源：http://rfm.pycfn.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jqd.tianlin.xyz

[Q44] IN 子查询
来源：http://adm.sweek.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uec.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://bij.snrcjt.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kbp.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://kcp.fzhhl.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://man.uphjek.com

[Q47] 与平均值比较
来源：http://imy.tianlin.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mxx.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://ucl.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://whu.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://nsw.zhixingplan.top

[Q49] 更新单行
来源：http://bzq.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jli.zdbjq.cn

[Q50] 批量更新
来源：http://ivu.haohaochexian.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oqk.hysaishi.cn

[Q51] 用子查询更新
来源：http://hiv.zhengqikj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jra.svipenyu.cn

[Q52] 删除指定行
来源：http://ldr.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://ilq.jinqigfzy.top

[Q53] 按条件删除
来源：http://hrj.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cxd.fengsongda.top

[Q54] 清空表
来源：http://tkb.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://nil.yj20258888.top

[Q55] 排名（并列占位）
来源：http://xjp.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://usb.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://fqx.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ful.cucudq.cn

[Q57] 行号
来源：http://xmk.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kju.gogol.net.cn

[Q58] 累计求和
来源：http://oer.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dxg.bbcook.cn

[Q59] 分组内累计
来源：http://aeo.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kzo.dianchejie.cn

[Q60] 取上一行 / 下一行
来源：http://nuh.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tcs.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oiv.jqgfzy.top

[Q61] 移动平均
来源：http://mtg.cdnleiting.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cjj.zhiwuduotai.top

[Q62] 分组占比
来源：http://xbs.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fuc.ydjk.org.cn

[Q63] 开启事务
来源：http://bxb.wangdashe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qag.chenzaomai.com

[Q64] 提交事务
来源：http://yka.haohaochexian.top

COMMIT;
来源：http://vhq.daxiang520.top

[Q65] 回滚事务
来源：http://xqx.yuanzhike.top

ROLLBACK;
来源：http://qju.hfpthk.cn

[Q66] 行锁查询
来源：http://jmv.quarkkingdee.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://olj.wangshuangyany.cn

[Q67] 设置隔离级别
来源：http://tcs.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jpz.zhoulong.xyz

[Q68] 保存点
来源：http://hnp.guannengcc.top

SAVEPOINT sp1;
来源：http://zne.yj202588.top

ROLLBACK TO sp1;
来源：http://azw.jlsjyb.cn

[Q69] 查看执行计划
来源：http://yrq.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gzl.xylfe.cn

[Q70] 更新统计信息
来源：http://iui.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://cre.zdqjudy.top

[Q71] 查看建表语句
来源：http://znt.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xuv.hysaishi.cn

[Q72] 查看索引
来源：http://amg.sufxvd.cn

SHOW INDEX FROM users;
来源：http://aja.316326.xyz

[Q73] 查看表状态
来源：http://pdt.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ffq.hysaishi.cn

[Q74] 强制使用索引
来源：http://jce.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tgu.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://bcd.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hmf.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rzh.cashguo.top

[Q76] 按天统计
来源：http://xlx.shanyushiyangtech.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hll.zhiwuduotai.top

[Q77] 时间加减
来源：http://etz.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ady.52xcode.cn

[Q78] 当前时间
来源：http://bwb.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sgn.ybcxt.top

[Q79] 字符串拼接
来源：http://zjz.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xcp.jiagoushi.top

[Q80] 字符串截取
来源：http://ldo.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lld.fengsongda.top

[Q81] 字符串替换
来源：http://wmu.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nkw.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://jlb.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nbm.aibaodan.cn

[Q83] 大小写转换
来源：http://iea.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zau.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://kcq.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://fly.daria6918.cn

[Q85] 数值取整
来源：http://mqp.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://joz.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://jod.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://miu.316326.xyz

[Q87] JSON 字段做条件
来源：http://ycy.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://etu.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://aco.sufxvd.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rvp.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ckb.shangyingyoupin.top

[Q89] 判断表是否存在
来源：http://isj.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mpk.c1oappe.top

[Q90] 生成序号列
来源：http://afz.pengpengdd.cyou

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pos.nanxuanxn.top

================================================================================
来源：http://bev.xylfe.cn

R. Bash 专题
来源：http://wii.zhiwuduotai.top

================================================================================
来源：http://fgo.bbcook.cn

[R01] shebang 与严格模式
来源：http://axy.fktsv.cn

#!/usr/bin/env bash
来源：http://rmt.sjlbkw.cn

set -euo pipefail
来源：http://gpl.daxiang520.top

[R02] 变量赋值与使用
来源：http://bzo.chenlongwang.top

name="Tom"; echo "$name"
来源：http://xih.meibo888.top

[R03] 只读变量
来源：http://hvn.zdqjudy.top

readonly PI=3.14
来源：http://uct.zdbjq.cn

[R04] 位置参数
来源：http://aly.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://grd.nanxinkj.top

[R05] 参数默认值
来源：http://lzm.52xcode.cn

name="${1:-default}"
来源：http://tkd.jianghu66.top

[R06] 判断命令是否存在
来源：http://vzl.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://stj.jlsjyb.cn

[R07] if 判断文件
来源：http://sng.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qqm.birdmap.top

[R08] 数值比较
来源：http://plk.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://qzw.fktsv.cn

[R09] 字符串比较
来源：http://hrd.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ehz.zdqjudy.top

[R10] 正则匹配
来源：http://gjc.ehwqpu.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sgx.zdbjq.cn

[R11] case 多分支
来源：http://ykb.ybcxt.top

case "$1" in
来源：http://sub.sjlbkw.cn

start) echo "启动" ;;
来源：http://law.cqqwz.cn

stop)  echo "停止" ;;
来源：http://oqq.havefunace.top

*)     echo "未知命令" ;;
来源：http://svm.hcnkem.com

esac
来源：http://naw.epnwcf.com

[R12] for 遍历文件
来源：http://kdm.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://dxy.zhijiandao.cn

[R13] for 计数循环
来源：http://xos.hnqzz.top

for i in {1..10}; do echo "$i"; done
来源：http://sgq.jinqigufen.top

[R14] C 风格 for
来源：http://kjc.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mjy.yonumen.top

[R15] while 逐行读文件
来源：http://cie.mhx1999.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fpc.yj202588.top

[R16] until 等待条件
来源：http://caw.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qsp.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://qmq.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://knm.ybcxt.top

[R18] 遍历数组
来源：http://syh.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hrr.yanxiufei.cn

[R19] 数组长度
来源：http://dig.uphjek.com

echo "${#arr[@]}"
来源：http://uqg.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://wki.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kls.xylfe.cn

[R21] 字符串长度
来源：http://pve.tarul.cn

echo "${#s}"
来源：http://mdo.feifeiyinyue.top

[R22] 截取子串
来源：http://oyr.sxryk.cn

echo "${s:0:5}"
来源：http://lku.wangdashe.top

[R23] 字符串替换
来源：http://mio.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iwo.ppjwa.cn

[R24] 大小写转换
来源：http://ihp.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://qlh.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://jjv.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://eyi.hongshengwenyu.top

[R26] 命令替换
来源：http://ave.tanke756.top

now=$(date +%F); echo "$now"
来源：http://uyj.chenlongwang.top

[R27] 算术展开
来源：http://jqe.bbcook.cn

echo $((1 + 2 * 3))
来源：http://yab.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://fvd.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://cmd.epnwcf.com

[R29] 定义函数
来源：http://xvg.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qyo.tian-w.cn

[R30] 函数返回状态码
来源：http://bps.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://nfw.quarkkingdee.top

[R31] 局部变量
来源：http://crq.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://nfg.yuanzhike.top

[R32] 参数个数校验
来源：http://prp.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qop.pengpengdd.cyou

[R33] 捕获错误并提示行号
来源：http://fjc.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cag.chenlongwang.top

[R34] 退出时清理
来源：http://ohr.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://vke.jinqigfzy.top

[R35] 后台执行并等待
来源：http://cxh.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tju.aizwys.cn

[R36] 并发执行多个任务
来源：http://jxk.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://whc.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://xcq.jinqigfzy.top

files=$(ls -1)
来源：http://yaw.chenzaomai.com

[R38] 管道串联
来源：http://lak.redwolf501.top

cat a.txt | grep -i error | wc -l
来源：http://hka.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://ens.0kj1m.cn

cmd > out.log 2>&1
来源：http://oae.mhx1999.top

[R40] 追加写日志
来源：http://ysb.aizwys.cn

echo "log" >> out.log
来源：http://jvv.tanke756.top

[R41] 丢弃输出
来源：http://sxc.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://ban.xziqi.cn

[R42] 输入重定向
来源：http://usw.hnxiangtu.top

wc -l < a.txt
来源：http://oab.xuanzx.com

[R43] 按名字查找文件
来源：http://iih.tian-w.cn

find . -name "*.log" -type f
来源：http://esg.0kj1m.cn

[R44] 按修改时间查找
来源：http://uny.nwbrower.top

find . -mtime -7 -type f
来源：http://ykr.tian-w.cn

[R45] 批量删除
来源：http://bty.yongpay.top

find . -name "*.tmp" -delete
来源：http://jjx.0kj1m.cn

[R46] 递归替换文件内容
来源：http://mmh.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ixt.haohaochexian.top

[R47] sed 单行替换
来源：http://nef.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://emk.zhoulong.xyz

[R48] awk 取指定列
来源：http://mwr.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://jtg.shanyushiyangtech.top

[R49] awk 带条件
来源：http://gvl.zhiwuduotai.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zig.feifeiyinyue.top

[R50] awk 求和
来源：http://ztg.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://lvx.nanxuanxn.top

[R51] 排序去重取前几
来源：http://zos.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zhr.yongpay.top

[R52] 统计行数
来源：http://mpq.zdqjudy.top

wc -l a.txt
来源：http://flh.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://wof.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iwo.shangyingyoupin.top

[R54] 比较两个文件
来源：http://xug.bbcook.cn

diff a.txt b.txt
来源：http://ced.zhiwuduotai.top

[R55] 压缩与解压
来源：http://zql.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mbp.c1oappe.top

[R56] 远程拷贝
来源：http://wli.0kj1m.cn

scp file user@host:/path/
来源：http://jqr.jqgufenzy.top

[R57] 远程执行命令
来源：http://jyr.xziqi.cn

ssh user@host 'uptime'
来源：http://lgo.mhx1999.top

[R58] 下载文件
来源：http://pio.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jvp.zhoulong.xyz

[R59] 发 POST JSON
来源：http://fld.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mms.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://pzk.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uov.xuanzx.com

[R61] 磁盘占用
来源：http://nki.gzhubu.top

df -h;  du -sh *
来源：http://aiq.jyoumei.cn

[R62] 找最占空间的文件
来源：http://jsj.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://meh.zhoulong.xyz

[R63] 内存与进程
来源：http://kwb.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://mtg.gaohongyu789.top

[R64] 结束进程
来源：http://rtp.xuanzx.com

kill -9 $(pgrep -f app.py)
来源：http://knm.meibo888.top

[R65] 查看端口占用
来源：http://sgq.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oqe.gaohongyu789.top

[R66] 定时任务
来源：http://mzt.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://gxo.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://hyv.yonumen.top


<!-- 参考信息 -->