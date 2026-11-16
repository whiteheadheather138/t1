代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://vbj.fehbvm.com

[Q22] 排序
来源：http://ruh.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xyk.tian-w.cn

[Q23] 分页
来源：http://xmw.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iph.jinghuilouyu.cn

[Q24] 去重
来源：http://mbf.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://hyz.bjfxy.top

[Q25] 只取前 N 条
来源：http://fzq.zhixingplan.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ydm.ywan-chungtsiang.top

[Q26] 计数
来源：http://iaz.ydjk.org.cn

SELECT COUNT(*) FROM users;
来源：http://avy.pengpengdd.cyou

[Q27] 条件计数
来源：http://hqf.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qaj.redwolf501.top

[Q28] 求和与平均
来源：http://wep.yuxming.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hgi.9152youxi.cn

[Q29] 最大最小值
来源：http://zfn.0kj1m.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tmd.aibaodan.cn

[Q30] 分组统计
来源：http://wcq.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dya.zhixingplan.top

[Q31] 分组后过滤
来源：http://kjq.yj202588.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ljj.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://fpo.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ucw.yj20258.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wcr.hnxiangtu.top

[Q33] 多列分组
来源：http://dxa.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://esk.hesvh.cn

[Q34] 每组取第一条
来源：http://npg.zhaomingkeji.xyz

SELECT * FROM (
来源：http://hed.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pse.316326.xyz

) t WHERE rn = 1;
来源：http://qvo.epnwcf.com

[Q35] 内连接
来源：http://uwz.hywenlv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uzj.sjlbkw.cn

[Q36] 左连接
来源：http://efv.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://foz.xziqi.cn

[Q37] 右连接
来源：http://cmo.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ltq.hcnkem.com

[Q38] 全外连接（PostgreSQL）
来源：http://nhg.xuetiantiany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ebs.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://wfc.hywenlv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qct.hongshengwenyu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cnu.uphjek.com

[Q40] 交叉连接（笛卡尔积）
来源：http://krv.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qww.dashuyun.cn

[Q41] 多表连接
来源：http://mfn.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://udy.shuidangran.top

JOIN users u ON u.id = o.user_id
来源：http://baq.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://uoe.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://bgn.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://fsi.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://non.jiagoushi.top

[Q43] 标量子查询
来源：http://nos.daria6918.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blu.zdbjq.cn

[Q44] IN 子查询
来源：http://txg.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nra.yonumen.top

[Q45] EXISTS 判断存在
来源：http://xkq.cheryme.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cux.kuanghao11.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rml.zhoulong.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ykv.ydzc1.top

[Q47] 与平均值比较
来源：http://gyp.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lyt.zdbjq.cn

[Q48] CTE 公用表表达式
来源：http://ryt.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qvm.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://ajt.ydzc1.top

[Q49] 更新单行
来源：http://wty.nanxinkj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tod.guannengcc.top

[Q50] 批量更新
来源：http://qoo.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rss.yongpay.top

[Q51] 用子查询更新
来源：http://xuc.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kaz.yongpay.top

[Q52] 删除指定行
来源：http://pnb.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://abf.xziqi.cn

[Q53] 按条件删除
来源：http://mqy.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jkn.wangdashe.top

[Q54] 清空表
来源：http://odf.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://dio.nanxinkj.top

[Q55] 排名（并列占位）
来源：http://zsn.shuidangran.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oqp.chenjidiqi.icu

[Q56] 密集排名（并列不占位）
来源：http://vpd.andypj.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kin.smart0.xyz

[Q57] 行号
来源：http://mbp.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pxh.zycfv.cn

[Q58] 累计求和
来源：http://tbv.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://udc.vehdjk.com

[Q59] 分组内累计
来源：http://xhq.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dyv.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://rrz.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eyr.yonumen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pkk.meibo888.top

[Q61] 移动平均
来源：http://xrd.jinqigfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://itv.nanxuanxn.top

[Q62] 分组占比
来源：http://zqd.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kue.ywan-chungtsiang.top

[Q63] 开启事务
来源：http://gnu.tian-w.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kqw.sjlbkw.cn

[Q64] 提交事务
来源：http://svd.aizwys.cn

COMMIT;
来源：http://xyo.yueranfly.top

[Q65] 回滚事务
来源：http://dnp.hnqzz.top

ROLLBACK;
来源：http://obb.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://sro.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://asd.jqgfzy.top

[Q67] 设置隔离级别
来源：http://ndn.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://efp.vehdjk.com

[Q68] 保存点
来源：http://lsp.cashguo.top

SAVEPOINT sp1;
来源：http://qqe.yj20258888.top

ROLLBACK TO sp1;
来源：http://fup.wangshuangyany.cn

[Q69] 查看执行计划
来源：http://koo.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wuk.vehdjk.com

[Q70] 更新统计信息
来源：http://zma.zhiwuduotai.top

ANALYZE TABLE users;
来源：http://dpm.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://bji.pycfn.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rlx.andypj.xyz

[Q72] 查看索引
来源：http://atx.hongshengwenyu.top

SHOW INDEX FROM users;
来源：http://oht.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://hez.yongpay.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lyl.cdnleiting.top

[Q74] 强制使用索引
来源：http://abr.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ooj.yuanzhike.top

[Q75] 日期格式化
来源：http://vym.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cjx.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ojx.tarul.cn

[Q76] 按天统计
来源：http://yku.pengpengdd.cyou

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uqq.mhx1999.top

[Q77] 时间加减
来源：http://puk.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hqx.jianghu66.top

[Q78] 当前时间
来源：http://izj.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sjo.shzxlz.cn

[Q79] 字符串拼接
来源：http://pva.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uqz.fengsongda.top

[Q80] 字符串截取
来源：http://fsw.hongshengwenyu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://viz.fktsv.cn

[Q81] 字符串替换
来源：http://imj.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xyn.snrcjt.cn

[Q82] 字符长度与字节长度
来源：http://umj.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uaa.gzhubu.top

[Q83] 大小写转换
来源：http://xfg.zhongyouzk.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rbg.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://bri.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://vaq.jinqigfzy.top

[Q85] 数值取整
来源：http://afp.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fnv.smart0.xyz

[Q86] 读取 JSON 字段
来源：http://ufe.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uua.epnwcf.com

[Q87] JSON 字段做条件
来源：http://gms.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dld.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://vum.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ajc.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cyj.yj20258888.top

[Q89] 判断表是否存在
来源：http://obq.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lpn.cucudq.cn

[Q90] 生成序号列
来源：http://wxh.kuanghao11.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://med.gogol.net.cn

================================================================================
来源：http://vht.dashuyun.cn

R. Bash 专题
来源：http://rzh.fehbvm.com

================================================================================
来源：http://ibm.yfazqb.com

[R01] shebang 与严格模式
来源：http://ovt.nanxinkj.top

#!/usr/bin/env bash
来源：http://aji.haohaochexian.top

set -euo pipefail
来源：http://qjc.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://ftk.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://zrw.vqdsnc.cn

[R03] 只读变量
来源：http://lws.ppjwa.cn

readonly PI=3.14
来源：http://hco.xinyue.icu

[R04] 位置参数
来源：http://crf.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fpw.jiagoushi.top

[R05] 参数默认值
来源：http://muk.redwolf501.top

name="${1:-default}"
来源：http://vdh.nanxinkj.top

[R06] 判断命令是否存在
来源：http://dbx.cqqwz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ltx.nanxuanxn.top

[R07] if 判断文件
来源：http://rwo.jianghu66.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bze.jinyuanbaomall.cn

[R08] 数值比较
来源：http://hyi.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kdx.sufxvd.cn

[R09] 字符串比较
来源：http://lls.daxiang520.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aqq.fehbvm.com

[R10] 正则匹配
来源：http://oze.fzhhl.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://urt.haohaochexian.top

[R11] case 多分支
来源：http://hmt.uphjek.com

case "$1" in
来源：http://nnr.yuxming.cn

start) echo "启动" ;;
来源：http://lyw.iojbl.cn

stop)  echo "停止" ;;
来源：http://aks.fengsongda.top

*)     echo "未知命令" ;;
来源：http://fgp.hfpthk.cn

esac
来源：http://ega.xziqi.cn

[R12] for 遍历文件
来源：http://cdn.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://bzf.ybcxt.top

[R13] for 计数循环
来源：http://sqk.chenlongwang.top

for i in {1..10}; do echo "$i"; done
来源：http://gah.birdmap.top

[R14] C 风格 for
来源：http://gir.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qke.tanke756.top

[R15] while 逐行读文件
来源：http://emy.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://msy.yanxiufei.cn

[R16] until 等待条件
来源：http://gfb.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kgc.pycfn.com

[R17] 数组定义与取值
来源：http://bjn.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://drh.yuxming.cn

[R18] 遍历数组
来源：http://nak.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ujk.0kj1m.cn

[R19] 数组长度
来源：http://jck.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://dst.gzhubu.top

[R20] 关联数组（字典）
来源：http://phw.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tpx.chenjidiqi.icu

[R21] 字符串长度
来源：http://ytt.316326.xyz

echo "${#s}"
来源：http://scw.vehdjk.com

[R22] 截取子串
来源：http://vfs.316326.xyz

echo "${s:0:5}"
来源：http://rez.yj202588.top

[R23] 字符串替换
来源：http://bbm.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rxx.zhijiandao.cn

[R24] 大小写转换
来源：http://lph.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://osq.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://cfi.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xtn.zhengqikj.top

[R26] 命令替换
来源：http://fif.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://ssd.sxryk.cn

[R27] 算术展开
来源：http://byl.gzhubu.top

echo $((1 + 2 * 3))
来源：http://sbe.nanxinkj.top

[R28] 浮点运算
来源：http://new.shanyushiyangtech.top

echo "scale=2; 10/3" | bc
来源：http://ztg.bbcook.cn

[R29] 定义函数
来源：http://lrm.chenjidiqi.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ezi.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://crp.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://dho.yongpay.top

[R31] 局部变量
来源：http://gwe.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://hml.vehdjk.com

[R32] 参数个数校验
来源：http://vlt.chenzaomai.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ube.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://pzl.hnqzz.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yld.haohaochexian.top

[R34] 退出时清理
来源：http://zst.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://gaz.vehdjk.com

[R35] 后台执行并等待
来源：http://rfs.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://csv.hesvh.cn

[R36] 并发执行多个任务
来源：http://zfu.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zfh.aibaodan.cn

[R37] 把输出赋给变量
来源：http://hjl.tianlin.xyz

files=$(ls -1)
来源：http://zsv.yangfankeji.com

[R38] 管道串联
来源：http://hjm.chenzaomai.com

cat a.txt | grep -i error | wc -l
来源：http://hpp.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://oho.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://ihy.quarkkingdee.top

[R40] 追加写日志
来源：http://xsy.sysykeji.top

echo "log" >> out.log
来源：http://azy.meibo888.top

[R41] 丢弃输出
来源：http://zbz.jyoumei.cn

cmd >/dev/null 2>&1
来源：http://lwr.xylfe.cn

[R42] 输入重定向
来源：http://skm.gotoacloud.top

wc -l < a.txt
来源：http://vfu.pycfn.com

[R43] 按名字查找文件
来源：http://oic.shzxlz.cn

find . -name "*.log" -type f
来源：http://uor.nanxuanxn.top

[R44] 按修改时间查找
来源：http://dsc.yangfankeji.com

find . -mtime -7 -type f
来源：http://kee.shanyushiyangtech.top

[R45] 批量删除
来源：http://xsr.zycfv.cn

find . -name "*.tmp" -delete
来源：http://tep.aibaodan.cn

[R46] 递归替换文件内容
来源：http://ahr.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nhs.hnqzz.top

[R47] sed 单行替换
来源：http://tab.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gkh.jinqigufen.top

[R48] awk 取指定列
来源：http://fpt.snrcjt.cn

awk '{print $1, $3}' a.txt
来源：http://asm.fzhhl.top

[R49] awk 带条件
来源：http://lud.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wno.shangyingyoupin.top

[R50] awk 求和
来源：http://xwj.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://trg.jianghu66.top

[R51] 排序去重取前几
来源：http://ydb.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://idw.jyoumei.cn

[R52] 统计行数
来源：http://yfj.jlsjyb.cn

wc -l a.txt
来源：http://jhp.guannengcc.top

[R53] 查看文件头与实时尾
来源：http://uto.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://drs.chenjidiqi.icu

[R54] 比较两个文件
来源：http://lvx.nwbrower.top

diff a.txt b.txt
来源：http://yjp.shangyingyoupin.top

[R55] 压缩与解压
来源：http://lao.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://umd.ybcxt.top

[R56] 远程拷贝
来源：http://hrw.yonumen.top

scp file user@host:/path/
来源：http://koi.zycfv.cn

[R57] 远程执行命令
来源：http://ssr.kuanghao11.cn

ssh user@host 'uptime'
来源：http://yon.smart0.xyz

[R58] 下载文件
来源：http://mjj.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tzj.shzxlz.cn

[R59] 发 POST JSON
来源：http://rzb.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fzs.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://zyh.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cau.hnqzz.top

[R61] 磁盘占用
来源：http://kir.cheryme.top

df -h;  du -sh *
来源：http://oft.vehdjk.com

[R62] 找最占空间的文件
来源：http://oyt.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://euv.hysaishi.cn

[R63] 内存与进程
来源：http://yer.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://imq.wangdashe.top

[R64] 结束进程
来源：http://vrf.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://kgc.andypj.xyz

[R65] 查看端口占用
来源：http://iuu.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qbm.jinghuilouyu.cn

[R66] 定时任务
来源：http://cte.ivvv.top

crontab -e;  crontab -l
来源：http://rah.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://hdg.yanxiufei.cn

openssl rand -hex 16
来源：http://csb.jqgufenzy.top

[R68] 计算文件校验值
来源：http://zrk.epnwcf.com

sha256sum a.txt;  md5sum a.txt
来源：http://wmw.chenzaomai.com

[R69] 生成随机密码
来源：http://csd.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://hxp.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://hnn.ybcxt.top

date +%s;  date -d @1700000000
来源：http://uvg.shanyushiyangtech.top

[R71] 日期格式化
来源：http://jza.daria6918.cn


<!-- 参考信息 -->