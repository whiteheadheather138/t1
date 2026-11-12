代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gep.gzhubu.top

[Q20] IN 列表
来源：http://uwt.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fjm.zycfv.cn

[Q21] 空值判断
来源：http://lrd.fengsongda.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ztj.cucudq.cn

[Q22] 排序
来源：http://wvr.jlsjyb.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dgz.ydzc1.top

[Q23] 分页
来源：http://ilz.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ojj.fehbvm.com

[Q24] 去重
来源：http://tqy.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://bqf.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://vop.dashuyun.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nrj.jqgfzy.top

[Q26] 计数
来源：http://fod.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://yql.haohaochexian.top

[Q27] 条件计数
来源：http://uec.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vxn.jyoumei.cn

[Q28] 求和与平均
来源：http://cze.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://agw.ehwqpu.com

[Q29] 最大最小值
来源：http://gso.xingfuxueyuan.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://qve.fengsongda.top

[Q30] 分组统计
来源：http://nas.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ewz.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://tke.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kjt.316326.xyz

[Q32] 分组拼接字符串
来源：http://pbv.jinghuilouyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cgs.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bsp.dashuyun.cn

[Q33] 多列分组
来源：http://pti.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dxn.cheryme.top

[Q34] 每组取第一条
来源：http://dpo.gaohongyu789.top

SELECT * FROM (
来源：http://eis.hnqzz.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qqh.jinyuanbaomall.cn

) t WHERE rn = 1;
来源：http://pzx.ppjwa.cn

[Q35] 内连接
来源：http://kgv.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mlf.jqgufenzy.top

[Q36] 左连接
来源：http://rbt.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mrd.gogol.net.cn

[Q37] 右连接
来源：http://fjw.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fza.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://snp.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ncl.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://izw.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xkp.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oxu.cqqwz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wcc.yueranfly.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zzz.gotoacloud.top

[Q41] 多表连接
来源：http://sjw.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wwq.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://bzb.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://wse.yonumen.top

[Q42] 连接条件附加过滤
来源：http://wgv.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://ogh.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dhk.uphjek.com

[Q43] 标量子查询
来源：http://psg.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hat.9152youxi.cn

[Q44] IN 子查询
来源：http://qmb.jqgfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xdl.fehbvm.com

[Q45] EXISTS 判断存在
来源：http://sfx.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kbf.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://hzy.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ovz.0kj1m.cn

[Q47] 与平均值比较
来源：http://uue.yj20258888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lgn.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://gyx.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kjf.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://wik.andypj.xyz

[Q49] 更新单行
来源：http://qfs.chenjidiqi.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lhr.gaohongyu789.top

[Q50] 批量更新
来源：http://fgn.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ggq.yonumen.top

[Q51] 用子查询更新
来源：http://dbb.epnwcf.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lto.316326.xyz

[Q52] 删除指定行
来源：http://qlr.sysykeji.top

DELETE FROM users WHERE id = 10;
来源：http://ohn.shangyingyoupin.top

[Q53] 按条件删除
来源：http://hnm.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nrf.sjlbkw.cn

[Q54] 清空表
来源：http://quu.tarul.cn

TRUNCATE TABLE logs;
来源：http://gbt.nanxuanxn.top

[Q55] 排名（并列占位）
来源：http://ryl.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yct.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://jnq.ppjwa.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yas.chenzaomai.com

[Q57] 行号
来源：http://fsl.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://swa.gaohongyu789.top

[Q58] 累计求和
来源：http://fqk.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bku.svipenyu.cn

[Q59] 分组内累计
来源：http://lij.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://org.iojbl.cn

[Q60] 取上一行 / 下一行
来源：http://loe.jianghu66.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bob.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wxh.sufxvd.cn

[Q61] 移动平均
来源：http://imy.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://frb.xuanzx.com

[Q62] 分组占比
来源：http://fsw.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wyi.xuanzx.com

[Q63] 开启事务
来源：http://mkc.ydjk.org.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yxn.sxryk.cn

[Q64] 提交事务
来源：http://loy.yuanzhike.top

COMMIT;
来源：http://yoq.yfazqb.com

[Q65] 回滚事务
来源：http://tbv.yuanzhike.top

ROLLBACK;
来源：http://qic.tanke756.top

[Q66] 行锁查询
来源：http://zhk.zhoulong.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://siz.ctjpmb.com

[Q67] 设置隔离级别
来源：http://loi.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bmh.yonumen.top

[Q68] 保存点
来源：http://jav.hywenlv.cn

SAVEPOINT sp1;
来源：http://nec.hnqzz.top

ROLLBACK TO sp1;
来源：http://mhl.yj202588.top

[Q69] 查看执行计划
来源：http://hhe.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rbs.hammf.cn

[Q70] 更新统计信息
来源：http://pwl.zhixingplan.top

ANALYZE TABLE users;
来源：http://gip.nanxuanxn.top

[Q71] 查看建表语句
来源：http://xjm.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cul.xinyue.icu

[Q72] 查看索引
来源：http://etu.shuidangran.top

SHOW INDEX FROM users;
来源：http://dln.shangyingyoupin.top

[Q73] 查看表状态
来源：http://vdl.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jsd.jyoumei.cn

[Q74] 强制使用索引
来源：http://mqf.gotoacloud.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wij.tian-w.cn

[Q75] 日期格式化
来源：http://jnz.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hpa.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tfm.hnqzz.top

[Q76] 按天统计
来源：http://sxm.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aqp.gzhubu.top

[Q77] 时间加减
来源：http://hkk.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jgz.c1oappe.top

[Q78] 当前时间
来源：http://sat.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sca.ivvv.top

[Q79] 字符串拼接
来源：http://btr.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qjl.yfazqb.com

[Q80] 字符串截取
来源：http://fvc.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vcv.0kj1m.cn

[Q81] 字符串替换
来源：http://cqd.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ucn.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://uou.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iea.sufxvd.cn

[Q83] 大小写转换
来源：http://evl.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jwc.shzxlz.cn

[Q84] 去除首尾空格
来源：http://uiv.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://zom.zhoulong.xyz

[Q85] 数值取整
来源：http://zzc.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vug.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://mtd.pengpengdd.cyou

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ywa.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://jub.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lma.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://nvu.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kpg.gogol.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cdi.sufxvd.cn

[Q89] 判断表是否存在
来源：http://fjg.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aqg.cheryme.top

[Q90] 生成序号列
来源：http://jlf.iojbl.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eis.pengpengdd.cyou

================================================================================
来源：http://nob.yuanzhike.top

R. Bash 专题
来源：http://ipx.andypj.xyz

================================================================================
来源：http://xkq.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://exy.daria6918.cn

#!/usr/bin/env bash
来源：http://day.shanyushiyangtech.top

set -euo pipefail
来源：http://ckn.jiagoushi.top

[R02] 变量赋值与使用
来源：http://hbr.yangfankeji.com

name="Tom"; echo "$name"
来源：http://fnd.fengsongda.top

[R03] 只读变量
来源：http://kzp.zhaomingkeji.xyz

readonly PI=3.14
来源：http://vao.guowangkeji.top

[R04] 位置参数
来源：http://saw.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mkv.haohaochexian.top

[R05] 参数默认值
来源：http://jhy.gaohongyu789.top

name="${1:-default}"
来源：http://cxx.zdqjudy.top

[R06] 判断命令是否存在
来源：http://gkm.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://spb.zhixingplan.top

[R07] if 判断文件
来源：http://ach.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cck.cheryme.top

[R08] 数值比较
来源：http://vqj.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://kgp.zdqjudy.top

[R09] 字符串比较
来源：http://gsi.nwbrower.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pjz.yuxming.cn

[R10] 正则匹配
来源：http://ktz.yonumen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://glp.nanxinkj.top

[R11] case 多分支
来源：http://rlt.wangshuangyany.cn

case "$1" in
来源：http://ieo.xingfuxueyuan.xyz

start) echo "启动" ;;
来源：http://lqm.yonumen.top

stop)  echo "停止" ;;
来源：http://lch.shuidangran.top

*)     echo "未知命令" ;;
来源：http://wpj.redwolf501.top

esac
来源：http://srz.sysykeji.top

[R12] for 遍历文件
来源：http://vpc.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://xrf.shangyingyoupin.top

[R13] for 计数循环
来源：http://wuy.gaohongyu789.top

for i in {1..10}; do echo "$i"; done
来源：http://zdh.tanke756.top

[R14] C 风格 for
来源：http://nuq.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gnq.ehwqpu.com

[R15] while 逐行读文件
来源：http://vrj.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rzd.cashguo.top

[R16] until 等待条件
来源：http://lyd.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yjo.gotoacloud.top

[R17] 数组定义与取值
来源：http://lhi.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://evm.zhiwuduotai.top

[R18] 遍历数组
来源：http://obp.xinyue.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bbx.xuanzx.com

[R19] 数组长度
来源：http://lzm.andypj.xyz

echo "${#arr[@]}"
来源：http://xya.wangdashe.top

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ogk.hnxiangtu.top

[R21] 字符串长度
来源：http://zsl.9152youxi.cn

echo "${#s}"
来源：http://sqf.smart0.xyz

[R22] 截取子串
来源：http://mlo.xuetiantiany.cn

echo "${s:0:5}"
来源：http://vgi.nwbrower.top

[R23] 字符串替换
来源：http://yxo.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ngk.quarkkingdee.top

[R24] 大小写转换
来源：http://rlb.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zms.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://sfp.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dhn.9152youxi.cn

[R26] 命令替换
来源：http://eoo.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://byj.gzhubu.top

[R27] 算术展开
来源：http://mqv.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://bvr.0kj1m.cn

[R28] 浮点运算
来源：http://cqf.cucudq.cn

echo "scale=2; 10/3" | bc
来源：http://pjy.chenlongwang.top

[R29] 定义函数
来源：http://xzb.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ogy.feifeiyinyue.top

[R30] 函数返回状态码
来源：http://ufk.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://krd.tarul.cn

[R31] 局部变量
来源：http://kfw.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://zkb.ctjpmb.com

[R32] 参数个数校验
来源：http://mkq.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://udz.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://usb.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lvo.ehwqpu.com

[R34] 退出时清理
来源：http://kcq.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://giv.zhiwuduotai.top

[R35] 后台执行并等待
来源：http://aqs.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uut.sweek.top

[R36] 并发执行多个任务
来源：http://vey.fzhhl.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rtv.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://rog.fengsongda.top

files=$(ls -1)
来源：http://jgk.hnqzz.top

[R38] 管道串联
来源：http://sjb.ehwqpu.com

cat a.txt | grep -i error | wc -l
来源：http://fep.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://rvf.ybcxt.top

cmd > out.log 2>&1
来源：http://sfw.xuanzx.com

[R40] 追加写日志
来源：http://loz.xingfuxueyuan.xyz

echo "log" >> out.log
来源：http://tnz.hywenlv.cn

[R41] 丢弃输出
来源：http://wvf.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://pjh.cqqwz.cn

[R42] 输入重定向
来源：http://vys.jqgfzy.top

wc -l < a.txt
来源：http://zjx.jinqigufen.top

[R43] 按名字查找文件
来源：http://ckk.xuanzx.com

find . -name "*.log" -type f
来源：http://fns.shzxlz.cn

[R44] 按修改时间查找
来源：http://jat.316326.xyz

find . -mtime -7 -type f
来源：http://trn.9152youxi.cn

[R45] 批量删除
来源：http://vla.cheryme.top

find . -name "*.tmp" -delete
来源：http://vco.cucudq.cn

[R46] 递归替换文件内容
来源：http://nyd.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ykc.vehdjk.com

[R47] sed 单行替换
来源：http://uwz.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://fea.andypj.xyz

[R48] awk 取指定列
来源：http://zdt.zhaomingkeji.xyz

awk '{print $1, $3}' a.txt
来源：http://lue.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://uec.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zbj.guowangkeji.top

[R50] awk 求和
来源：http://xbq.guannengcc.top

awk '{s += $2} END {print s}' a.txt
来源：http://vph.sufxvd.cn

[R51] 排序去重取前几
来源：http://jgs.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yyu.bjfxy.top

[R52] 统计行数
来源：http://vev.chenjidiqi.icu

wc -l a.txt
来源：http://ata.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://nhh.jianghu66.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wux.shanyushiyangtech.top

[R54] 比较两个文件
来源：http://vkc.hongshengwenyu.top

diff a.txt b.txt
来源：http://exq.hnxiangtu.top

[R55] 压缩与解压
来源：http://ewv.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hsq.fehbvm.com

[R56] 远程拷贝
来源：http://apc.zdbjq.cn

scp file user@host:/path/
来源：http://vhn.52xcode.cn

[R57] 远程执行命令
来源：http://tef.uphjek.com

ssh user@host 'uptime'
来源：http://jqc.kuanghao11.cn

[R58] 下载文件
来源：http://cmw.shanyushiyangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vtg.xinyue.icu

[R59] 发 POST JSON
来源：http://psk.xziqi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://joq.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://wnh.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uoi.zhiwuduotai.top

[R61] 磁盘占用
来源：http://mzc.jyoumei.cn

df -h;  du -sh *
来源：http://nzb.nanxinkj.top

[R62] 找最占空间的文件
来源：http://bic.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://bpb.bjfxy.top

[R63] 内存与进程
来源：http://elw.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://zdk.ydjk.org.cn

[R64] 结束进程
来源：http://mbo.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://uth.pengpengdd.cyou

[R65] 查看端口占用
来源：http://zbu.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://piw.shanyushiyangtech.top

[R66] 定时任务
来源：http://vev.dashuyun.cn

crontab -e;  crontab -l
来源：http://yqo.sysykeji.top

[R67] 生成随机十六进制串
来源：http://mfj.cdnleiting.top

openssl rand -hex 16
来源：http://zvy.gaohongyu789.top

[R68] 计算文件校验值
来源：http://xwc.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://obf.quarkkingdee.top

[R69] 生成随机密码
来源：http://nuf.nwbrower.top


<!-- 参考信息 -->