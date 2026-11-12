代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://zsj.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qpt.ivvv.top

[Q39] 自连接（查上下级）
来源：http://heg.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://rph.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qia.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vky.aizwys.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ttn.shangyingyoupin.top

[Q41] 多表连接
来源：http://jxo.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uka.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://knl.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://sbj.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://lss.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://ple.hesvh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ctp.jinqigfzy.top

[Q43] 标量子查询
来源：http://riw.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uph.ctjpmb.com

[Q44] IN 子查询
来源：http://cao.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rou.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://oxr.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gsf.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://wib.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qjj.cucudq.cn

[Q47] 与平均值比较
来源：http://jrd.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hvj.zhixingplan.top

[Q48] CTE 公用表表达式
来源：http://lyd.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pzv.zhoulong.xyz

SELECT * FROM t WHERE c > 5;
来源：http://bwp.cucudq.cn

[Q49] 更新单行
来源：http://kdo.zycfv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://syh.hnqzz.top

[Q50] 批量更新
来源：http://cjw.sysykeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uyl.zhijiandao.cn

[Q51] 用子查询更新
来源：http://lzl.shangyingyoupin.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://imx.cashguo.top

[Q52] 删除指定行
来源：http://tay.zhixingplan.top

DELETE FROM users WHERE id = 10;
来源：http://osi.jqgufenzy.top

[Q53] 按条件删除
来源：http://cyl.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jth.jianghu66.top

[Q54] 清空表
来源：http://tmf.xuetiantiany.cn

TRUNCATE TABLE logs;
来源：http://rfm.mhx1999.top

[Q55] 排名（并列占位）
来源：http://kqu.hysaishi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jfi.shanyushiyangtech.top

[Q56] 密集排名（并列不占位）
来源：http://hgy.aibaodan.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kvr.ydjk.org.cn

[Q57] 行号
来源：http://rco.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hot.gaohongyu789.top

[Q58] 累计求和
来源：http://amg.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tyv.zhongyouzk.top

[Q59] 分组内累计
来源：http://net.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pgj.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://pqe.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lfy.yj20258888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pgt.wangshuangyany.cn

[Q61] 移动平均
来源：http://wlr.jqgufenzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fap.nanxuanxn.top

[Q62] 分组占比
来源：http://uao.ydzc1.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qvz.tianlin.xyz

[Q63] 开启事务
来源：http://mjx.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ewx.birdmap.top

[Q64] 提交事务
来源：http://fen.cheryme.top

COMMIT;
来源：http://ker.andypj.xyz

[Q65] 回滚事务
来源：http://oww.wangshuangyany.cn

ROLLBACK;
来源：http://yiu.hfpthk.cn

[Q66] 行锁查询
来源：http://grf.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xiz.fzhhl.top

[Q67] 设置隔离级别
来源：http://csb.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nhs.zdbjq.cn

[Q68] 保存点
来源：http://vlt.xziqi.cn

SAVEPOINT sp1;
来源：http://jaj.hesvh.cn

ROLLBACK TO sp1;
来源：http://tzb.tianlin.xyz

[Q69] 查看执行计划
来源：http://jta.gaohongyu789.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rmx.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://tno.jianghu66.top

ANALYZE TABLE users;
来源：http://rke.uphjek.com

[Q71] 查看建表语句
来源：http://bhc.havefunace.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ubz.jlsjyb.cn

[Q72] 查看索引
来源：http://xgm.nanxinkj.top

SHOW INDEX FROM users;
来源：http://xjp.hysaishi.cn

[Q73] 查看表状态
来源：http://osq.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://liv.zhongyouzk.top

[Q74] 强制使用索引
来源：http://san.hongshengwenyu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wfd.jyoumei.cn

[Q75] 日期格式化
来源：http://nke.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lvk.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://woa.uphjek.com

[Q76] 按天统计
来源：http://ift.hnxiangtu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bhx.xingfuxueyuan.xyz

[Q77] 时间加减
来源：http://rdt.jyoumei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nii.yuxming.cn

[Q78] 当前时间
来源：http://crt.fehbvm.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hqv.ybcxt.top

[Q79] 字符串拼接
来源：http://dre.jinyuanbaomall.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sdr.9152youxi.cn

[Q80] 字符串截取
来源：http://grw.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ssg.yuanzhike.top

[Q81] 字符串替换
来源：http://adj.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ivw.dianchejie.cn

[Q82] 字符长度与字节长度
来源：http://fkk.iojbl.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://szj.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://icu.jianghu66.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jah.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://dan.havefunace.top

SELECT TRIM(name) FROM users;
来源：http://mky.cashguo.top

[Q85] 数值取整
来源：http://wzp.gotoacloud.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xpu.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://cmt.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vlo.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://lxf.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ole.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://nvc.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vtv.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uat.chenlongwang.top

[Q89] 判断表是否存在
来源：http://zvk.316326.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://juz.xuanzx.com

[Q90] 生成序号列
来源：http://xzi.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://riq.yueranfly.top

================================================================================
来源：http://gvr.yongpay.top

R. Bash 专题
来源：http://xdi.kuanghao11.cn

================================================================================
来源：http://kny.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://keb.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://ldq.aibaodan.cn

set -euo pipefail
来源：http://ygy.aibaodan.cn

[R02] 变量赋值与使用
来源：http://nro.yuxming.cn

name="Tom"; echo "$name"
来源：http://ykn.yj20258888.top

[R03] 只读变量
来源：http://gfe.aizwys.cn

readonly PI=3.14
来源：http://kwy.meibo888.top

[R04] 位置参数
来源：http://poz.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ujl.ehwqpu.com

[R05] 参数默认值
来源：http://qyb.epnwcf.com

name="${1:-default}"
来源：http://hgz.jinqigufen.top

[R06] 判断命令是否存在
来源：http://alr.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://twe.birdmap.top

[R07] if 判断文件
来源：http://ppw.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bxs.birdmap.top

[R08] 数值比较
来源：http://scp.daxiang520.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uzm.fengsongda.top

[R09] 字符串比较
来源：http://enp.hnxiangtu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hiu.ivvv.top

[R10] 正则匹配
来源：http://ytf.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pak.xinyue.icu

[R11] case 多分支
来源：http://zrn.iojbl.cn

case "$1" in
来源：http://raw.iojbl.cn

start) echo "启动" ;;
来源：http://bql.yangfankeji.com

stop)  echo "停止" ;;
来源：http://gvo.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://tpo.nanxuanxn.top

esac
来源：http://cqa.cdnleiting.top

[R12] for 遍历文件
来源：http://vao.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://lom.cheryme.top

[R13] for 计数循环
来源：http://nmz.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://rkr.zhixingplan.top

[R14] C 风格 for
来源：http://sqk.ivvv.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dwv.epnwcf.com

[R15] while 逐行读文件
来源：http://bxl.aibaodan.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rzq.redwolf501.top

[R16] until 等待条件
来源：http://oop.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sin.kuanghao11.cn

[R17] 数组定义与取值
来源：http://lyo.birdmap.top

arr=(a b c); echo "${arr[0]}"
来源：http://pkq.hnqzz.top

[R18] 遍历数组
来源：http://uyo.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lis.hnqzz.top

[R19] 数组长度
来源：http://ayh.bjfxy.top

echo "${#arr[@]}"
来源：http://zow.jyoumei.cn

[R20] 关联数组（字典）
来源：http://psg.gzhubu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vvp.snrcjt.cn

[R21] 字符串长度
来源：http://joo.zdbjq.cn

echo "${#s}"
来源：http://ygv.cdnleiting.top

[R22] 截取子串
来源：http://bgm.kuanghao11.cn

echo "${s:0:5}"
来源：http://llk.yj20258.top

[R23] 字符串替换
来源：http://hpg.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://feb.zycfv.cn

[R24] 大小写转换
来源：http://van.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://gtt.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://ngm.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ufu.sjlbkw.cn

[R26] 命令替换
来源：http://yad.hfpthk.cn

now=$(date +%F); echo "$now"
来源：http://iom.jianghu66.top

[R27] 算术展开
来源：http://dnn.zdqjudy.top

echo $((1 + 2 * 3))
来源：http://xjw.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://dsf.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://jms.cashguo.top

[R29] 定义函数
来源：http://qsg.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ftk.xylfe.cn

[R30] 函数返回状态码
来源：http://ohe.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://fje.xuetiantiany.cn

[R31] 局部变量
来源：http://cab.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://tvh.mhx1999.top

[R32] 参数个数校验
来源：http://qeg.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tfc.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://htq.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zgn.havefunace.top

[R34] 退出时清理
来源：http://lpu.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://abz.tanke756.top

[R35] 后台执行并等待
来源：http://knc.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://qzs.ybcxt.top

[R36] 并发执行多个任务
来源：http://asb.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dog.chenlongwang.top

[R37] 把输出赋给变量
来源：http://jps.sjlbkw.cn

files=$(ls -1)
来源：http://ddf.guowangkeji.top

[R38] 管道串联
来源：http://nzu.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://flk.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://byd.ppjwa.cn

cmd > out.log 2>&1
来源：http://ina.hywenlv.cn

[R40] 追加写日志
来源：http://ruh.hcnkem.com

echo "log" >> out.log
来源：http://uza.xinyue.icu

[R41] 丢弃输出
来源：http://aka.tianlin.xyz

cmd >/dev/null 2>&1
来源：http://odi.zdqjudy.top

[R42] 输入重定向
来源：http://oze.birdmap.top

wc -l < a.txt
来源：http://vkh.jqgfzy.top

[R43] 按名字查找文件
来源：http://jbr.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://eud.cashguo.top

[R44] 按修改时间查找
来源：http://vip.yj202588.top

find . -mtime -7 -type f
来源：http://uxl.vehdjk.com

[R45] 批量删除
来源：http://doa.pengpengdd.cyou

find . -name "*.tmp" -delete
来源：http://itj.yj20258.top

[R46] 递归替换文件内容
来源：http://mob.jlsjyb.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dgm.fktsv.cn

[R47] sed 单行替换
来源：http://qca.tian-w.cn

sed -i 's/foo/bar/g' a.txt
来源：http://unp.52xcode.cn

[R48] awk 取指定列
来源：http://lel.mhx1999.top

awk '{print $1, $3}' a.txt
来源：http://exv.jinghuilouyu.cn

[R49] awk 带条件
来源：http://qog.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wfp.jinyuanbaomall.cn

[R50] awk 求和
来源：http://edc.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://udr.0kj1m.cn

[R51] 排序去重取前几
来源：http://bgc.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ffr.vqdsnc.cn

[R52] 统计行数
来源：http://krc.yj20258.top

wc -l a.txt
来源：http://cad.tianlin.xyz

[R53] 查看文件头与实时尾
来源：http://nxg.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wck.shzxlz.cn

[R54] 比较两个文件
来源：http://lim.cashguo.top

diff a.txt b.txt
来源：http://fxh.ydjk.org.cn

[R55] 压缩与解压
来源：http://gzg.daxiang520.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sqh.ehwqpu.com

[R56] 远程拷贝
来源：http://ptw.ybcxt.top

scp file user@host:/path/
来源：http://zum.tanke756.top

[R57] 远程执行命令
来源：http://rtl.aibaodan.cn

ssh user@host 'uptime'
来源：http://qvm.fktsv.cn

[R58] 下载文件
来源：http://twd.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ult.xinyue.icu

[R59] 发 POST JSON
来源：http://hwp.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bwo.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://ymv.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eox.shzxlz.cn

[R61] 磁盘占用
来源：http://bzh.yonumen.top

df -h;  du -sh *
来源：http://knl.fengsongda.top

[R62] 找最占空间的文件
来源：http://wio.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://utg.ehwqpu.com

[R63] 内存与进程
来源：http://exc.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://fxt.52xcode.cn

[R64] 结束进程
来源：http://dbm.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://bjy.hesvh.cn

[R65] 查看端口占用
来源：http://joe.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ist.guowangkeji.top

[R66] 定时任务
来源：http://xtw.chenlongwang.top

crontab -e;  crontab -l
来源：http://dei.daria6918.cn

[R67] 生成随机十六进制串
来源：http://jkl.yanxiufei.cn

openssl rand -hex 16
来源：http://wnk.aizwys.cn

[R68] 计算文件校验值
来源：http://tbp.jlsjyb.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dld.nwbrower.top

[R69] 生成随机密码
来源：http://fkb.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://ilu.shuidangran.top

[R70] 时间戳与互转
来源：http://sqq.bbcook.cn

date +%s;  date -d @1700000000
来源：http://yev.zhixingplan.top

[R71] 日期格式化
来源：http://lww.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://oyy.jqgufenzy.top

[R72] 等待端口就绪
来源：http://thx.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bvo.xinyue.icu

[R73] 分割大日志
来源：http://lpe.sweek.top

split -l 1000 big.log part_
来源：http://tpr.jianghu66.top

[R74] 批量重命名
来源：http://eat.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://itd.tianlin.xyz

[R75] 导出环境变量
来源：http://npv.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://htm.fktsv.cn

[R76] 使用临时文件
来源：http://fmt.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xyg.gogol.net.cn

[R77] 读取用户输入
来源：http://uqu.zhoulong.xyz

read -rp "请输入: " ans
来源：http://afe.guannengcc.top

[R78] 交互式菜单
来源：http://okg.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gnd.nwbrower.top

[R79] 解析命令行选项
来源：http://izt.yueranfly.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hje.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://fwf.snrcjt.cn

time ./run.sh
来源：http://dds.sweek.top

================================================================================
来源：http://bzb.316326.xyz

S. C / C++ 专题
来源：http://dkj.xinyue.icu

================================================================================
来源：http://ojy.uphjek.com

[S01] C：Hello World
来源：http://ijo.cdnleiting.top

#include <stdio.h>
来源：http://beq.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hxi.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://nxa.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://fuy.0kj1m.cn

[S03] C：读入整数
来源：http://skx.yfazqb.com

int x; scanf("%d", &x);
来源：http://vhc.zhijiandao.cn

[S04] C：字符串复制
来源：http://zak.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://kgg.xuanzx.com

[S05] C：字符串长度
来源：http://uyw.yangfankeji.com

strlen(s)
来源：http://alj.hammf.cn

[S06] C：字符串比较
来源：http://rgu.0kj1m.cn

strcmp(a, b) == 0
来源：http://ukb.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://xxj.guannengcc.top


<!-- 参考信息 -->