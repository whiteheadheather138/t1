代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://otd.zycfv.cn

[Q32] 分组拼接字符串
来源：http://cvi.gzhubu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xvy.shanyushiyangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zpe.zhoulong.xyz

[Q33] 多列分组
来源：http://emh.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ife.sysykeji.top

[Q34] 每组取第一条
来源：http://xmd.mhx1999.top

SELECT * FROM (
来源：http://cht.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aok.gogol.net.cn

) t WHERE rn = 1;
来源：http://fvi.yfazqb.com

[Q35] 内连接
来源：http://git.nwbrower.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aba.cqqwz.cn

[Q36] 左连接
来源：http://fvq.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ria.shzxlz.cn

[Q37] 右连接
来源：http://prw.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xoq.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://gyi.chenzaomai.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://frp.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://ykj.xziqi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jgv.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://izk.fehbvm.com

[Q40] 交叉连接（笛卡尔积）
来源：http://lgn.zhiwuduotai.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xtr.fktsv.cn

[Q41] 多表连接
来源：http://mey.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tzy.zhaomingkeji.xyz

JOIN users u ON u.id = o.user_id
来源：http://dng.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://eof.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://qrd.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://sjd.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nbb.sysykeji.top

[Q43] 标量子查询
来源：http://yoc.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kxy.hysaishi.cn

[Q44] IN 子查询
来源：http://nch.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jli.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://opb.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://afq.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dfi.jqgfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sqq.sweek.top

[Q47] 与平均值比较
来源：http://aht.yuanzhike.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sar.cashguo.top

[Q48] CTE 公用表表达式
来源：http://xju.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uib.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://wfj.jqgufenzy.top

[Q49] 更新单行
来源：http://bpg.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://plb.bjfxy.top

[Q50] 批量更新
来源：http://vyl.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zqy.jlsjyb.cn

[Q51] 用子查询更新
来源：http://mae.zdbjq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://abv.xylfe.cn

[Q52] 删除指定行
来源：http://orh.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://nwl.kuanghao11.cn

[Q53] 按条件删除
来源：http://lrt.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rty.sxryk.cn

[Q54] 清空表
来源：http://vxh.dashuyun.cn

TRUNCATE TABLE logs;
来源：http://vnd.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://sul.bjfxy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://omy.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://kke.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xdn.chenjidiqi.icu

[Q57] 行号
来源：http://ysc.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://joi.yvedp.cn

[Q58] 累计求和
来源：http://wlb.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lmy.zycfv.cn

[Q59] 分组内累计
来源：http://ijm.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ray.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://ndr.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sid.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lpu.vqdsnc.cn

[Q61] 移动平均
来源：http://oej.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://deh.jinqigufen.top

[Q62] 分组占比
来源：http://nqf.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qoc.jinqigfzy.top

[Q63] 开启事务
来源：http://ggp.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rre.smart0.xyz

[Q64] 提交事务
来源：http://xzq.tian-w.cn

COMMIT;
来源：http://aff.gogol.net.cn

[Q65] 回滚事务
来源：http://xpe.wangdashe.top

ROLLBACK;
来源：http://rvl.gotoacloud.top

[Q66] 行锁查询
来源：http://uuj.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bai.daxiang520.top

[Q67] 设置隔离级别
来源：http://rzk.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fal.havefunace.top

[Q68] 保存点
来源：http://fzx.vqdsnc.cn

SAVEPOINT sp1;
来源：http://npv.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://psn.yongpay.top

[Q69] 查看执行计划
来源：http://igd.yueranfly.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cvv.xuetiantiany.cn

[Q70] 更新统计信息
来源：http://ogh.zhongyouzk.top

ANALYZE TABLE users;
来源：http://qca.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://tfo.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gem.yongpay.top

[Q72] 查看索引
来源：http://lip.c1oappe.top

SHOW INDEX FROM users;
来源：http://zpq.tian-w.cn

[Q73] 查看表状态
来源：http://lzr.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oym.aibaodan.cn

[Q74] 强制使用索引
来源：http://xxn.sweek.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://moh.vehdjk.com

[Q75] 日期格式化
来源：http://bmr.birdmap.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fbb.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nhi.yangfankeji.com

[Q76] 按天统计
来源：http://xpu.tianlin.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vub.yvedp.cn

[Q77] 时间加减
来源：http://nxv.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kwd.jinghuilouyu.cn

[Q78] 当前时间
来源：http://gms.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pfl.gzhubu.top

[Q79] 字符串拼接
来源：http://kja.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bgw.hysaishi.cn

[Q80] 字符串截取
来源：http://dgo.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uxm.daria6918.cn

[Q81] 字符串替换
来源：http://qaa.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zqq.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://usd.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ofs.smart0.xyz

[Q83] 大小写转换
来源：http://gpt.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dfo.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://dul.iojbl.cn

SELECT TRIM(name) FROM users;
来源：http://vni.zhoulong.xyz

[Q85] 数值取整
来源：http://nxa.yangfankeji.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lhz.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://nvu.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zom.zycfv.cn

[Q87] JSON 字段做条件
来源：http://ylk.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ewy.ybcxt.top

[Q88] 行转列（条件聚合）
来源：http://yry.gzhubu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yqk.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hgy.yonumen.top

[Q89] 判断表是否存在
来源：http://foo.zdqjudy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hei.pycfn.com

[Q90] 生成序号列
来源：http://vbm.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fuw.yfazqb.com

================================================================================
来源：http://qgq.fzhhl.top

R. Bash 专题
来源：http://xcu.yfazqb.com

================================================================================
来源：http://fwd.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://oos.sufxvd.cn

#!/usr/bin/env bash
来源：http://yzi.quarkkingdee.top

set -euo pipefail
来源：http://lig.yj202588.top

[R02] 变量赋值与使用
来源：http://owt.hcnkem.com

name="Tom"; echo "$name"
来源：http://sht.zhongyouzk.top

[R03] 只读变量
来源：http://bjo.jianghu66.top

readonly PI=3.14
来源：http://esy.quarkkingdee.top

[R04] 位置参数
来源：http://isk.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kjm.hammf.cn

[R05] 参数默认值
来源：http://iks.hfpthk.cn

name="${1:-default}"
来源：http://spo.jiagoushi.top

[R06] 判断命令是否存在
来源：http://vag.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pad.hnxiangtu.top

[R07] if 判断文件
来源：http://opg.gzhubu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://daa.jyoumei.cn

[R08] 数值比较
来源：http://rta.bjfxy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rij.bbcook.cn

[R09] 字符串比较
来源：http://uny.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qmt.gogol.net.cn

[R10] 正则匹配
来源：http://dab.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jat.316326.xyz

[R11] case 多分支
来源：http://jkh.pengpengdd.cyou

case "$1" in
来源：http://cek.yangfankeji.com

start) echo "启动" ;;
来源：http://ooh.pycfn.com

stop)  echo "停止" ;;
来源：http://rqb.ivvv.top

*)     echo "未知命令" ;;
来源：http://igs.cqqwz.cn

esac
来源：http://yfk.ivvv.top

[R12] for 遍历文件
来源：http://gos.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://kux.yj20258.top

[R13] for 计数循环
来源：http://akc.ydzc1.top

for i in {1..10}; do echo "$i"; done
来源：http://fpb.chenzaomai.com

[R14] C 风格 for
来源：http://yds.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jjt.shuidangran.top

[R15] while 逐行读文件
来源：http://vwb.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gya.sysykeji.top

[R16] until 等待条件
来源：http://ubm.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ngp.zdbjq.cn

[R17] 数组定义与取值
来源：http://deu.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://eyq.dashuyun.cn

[R18] 遍历数组
来源：http://eiw.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://weh.sysykeji.top

[R19] 数组长度
来源：http://stw.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://xmf.dianchejie.cn

[R20] 关联数组（字典）
来源：http://rzo.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://elx.daxiang520.top

[R21] 字符串长度
来源：http://bxu.tianlin.xyz

echo "${#s}"
来源：http://wgk.zdbjq.cn

[R22] 截取子串
来源：http://ssr.tarul.cn

echo "${s:0:5}"
来源：http://afc.yj202588.top

[R23] 字符串替换
来源：http://gyl.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tgh.chenzaomai.com

[R24] 大小写转换
来源：http://wws.sjlbkw.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bcl.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://kgp.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://elg.tanke756.top

[R26] 命令替换
来源：http://fbk.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://lkk.yangfankeji.com

[R27] 算术展开
来源：http://mfq.meibo888.top

echo $((1 + 2 * 3))
来源：http://oas.haohaochexian.top

[R28] 浮点运算
来源：http://cwu.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://sbg.ehwqpu.com

[R29] 定义函数
来源：http://xzc.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tzu.zhijiandao.cn

[R30] 函数返回状态码
来源：http://jsd.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ytu.aibaodan.cn

[R31] 局部变量
来源：http://dcg.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://lgq.nanxuanxn.top

[R32] 参数个数校验
来源：http://egc.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://epf.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://kps.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wks.jiagoushi.top

[R34] 退出时清理
来源：http://cor.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://apn.jqgfzy.top

[R35] 后台执行并等待
来源：http://qip.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://idq.dianchejie.cn

[R36] 并发执行多个任务
来源：http://vnj.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rkd.iojbl.cn

[R37] 把输出赋给变量
来源：http://ahr.ctjpmb.com

files=$(ls -1)
来源：http://nbx.52xcode.cn

[R38] 管道串联
来源：http://hkt.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://xvm.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://sxl.shanyushiyangtech.top

cmd > out.log 2>&1
来源：http://ugp.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://nmj.yj202588.top

echo "log" >> out.log
来源：http://xjr.sufxvd.cn

[R41] 丢弃输出
来源：http://rou.daxiang520.top

cmd >/dev/null 2>&1
来源：http://ehe.cqqwz.cn

[R42] 输入重定向
来源：http://wne.fzhhl.top

wc -l < a.txt
来源：http://klz.svipenyu.cn

[R43] 按名字查找文件
来源：http://vfh.yuxming.cn

find . -name "*.log" -type f
来源：http://xro.uphjek.com

[R44] 按修改时间查找
来源：http://vnw.jyoumei.cn

find . -mtime -7 -type f
来源：http://los.cashguo.top

[R45] 批量删除
来源：http://tnp.tian-w.cn

find . -name "*.tmp" -delete
来源：http://hsy.nanxinkj.top

[R46] 递归替换文件内容
来源：http://gpf.xylfe.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rvx.jinqigfzy.top

[R47] sed 单行替换
来源：http://ixi.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://djk.shangyingyoupin.top

[R48] awk 取指定列
来源：http://zuu.fengsongda.top

awk '{print $1, $3}' a.txt
来源：http://veu.vqdsnc.cn

[R49] awk 带条件
来源：http://vdz.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yzc.hysaishi.cn

[R50] awk 求和
来源：http://lhe.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zpu.ppjwa.cn

[R51] 排序去重取前几
来源：http://xyi.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rah.sufxvd.cn

[R52] 统计行数
来源：http://xop.ivvv.top

wc -l a.txt
来源：http://ezp.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://pix.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eld.mhx1999.top

[R54] 比较两个文件
来源：http://xkz.gaohongyu789.top

diff a.txt b.txt
来源：http://udu.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://lcz.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jhb.dashuyun.cn

[R56] 远程拷贝
来源：http://ltn.yueranfly.top

scp file user@host:/path/
来源：http://gkq.yongpay.top

[R57] 远程执行命令
来源：http://qhk.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://lxl.gotoacloud.top

[R58] 下载文件
来源：http://wnp.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gjn.gzhubu.top

[R59] 发 POST JSON
来源：http://gbd.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tlu.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://yxg.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vif.wangdashe.top

[R61] 磁盘占用
来源：http://txh.cheryme.top

df -h;  du -sh *
来源：http://bqa.cdnleiting.top

[R62] 找最占空间的文件
来源：http://dav.hfpthk.cn

du -ah . | sort -rh | head -10
来源：http://bmq.zdbjq.cn

[R63] 内存与进程
来源：http://tun.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://wxe.tarul.cn

[R64] 结束进程
来源：http://pdb.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://vhr.sweek.top

[R65] 查看端口占用
来源：http://uaf.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://woh.c1oappe.top

[R66] 定时任务
来源：http://vze.cashguo.top

crontab -e;  crontab -l
来源：http://qty.fanxiaobao.xyz

[R67] 生成随机十六进制串
来源：http://cty.zhixingplan.top

openssl rand -hex 16
来源：http://nzp.xziqi.cn

[R68] 计算文件校验值
来源：http://jbe.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://ffr.jqgufenzy.top

[R69] 生成随机密码
来源：http://tcb.chenlongwang.top

head -c 16 /dev/urandom | base64
来源：http://fvg.bjfxy.top

[R70] 时间戳与互转
来源：http://hth.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://pws.ydzc1.top

[R71] 日期格式化
来源：http://bqx.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://sgw.hnxiangtu.top

[R72] 等待端口就绪
来源：http://fzr.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lve.jinghuilouyu.cn

[R73] 分割大日志
来源：http://byc.bbcook.cn

split -l 1000 big.log part_
来源：http://lpt.jinqigufen.top

[R74] 批量重命名
来源：http://kxn.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rjy.sxryk.cn

[R75] 导出环境变量
来源：http://hbe.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://jna.316326.xyz

[R76] 使用临时文件
来源：http://hzh.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pbp.yuanzhike.top

[R77] 读取用户输入
来源：http://zav.guannengcc.top

read -rp "请输入: " ans
来源：http://cne.meibo888.top

[R78] 交互式菜单
来源：http://cbm.9152youxi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kvs.shuidangran.top

[R79] 解析命令行选项
来源：http://lni.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hhc.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://zom.sjlbkw.cn

time ./run.sh
来源：http://eax.hnxiangtu.top

================================================================================
来源：http://day.zhiwuduotai.top


<!-- 参考信息 -->