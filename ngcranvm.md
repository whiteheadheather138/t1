代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://zbs.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wxa.jinqigfzy.top

[Q43] 标量子查询
来源：http://xye.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://frw.jqgufenzy.top

[Q44] IN 子查询
来源：http://acs.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fca.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://gys.zhiwuduotai.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jvm.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wiw.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vvi.zhijiandao.cn

[Q47] 与平均值比较
来源：http://fvk.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iag.tanke756.top

[Q48] CTE 公用表表达式
来源：http://jnb.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jgw.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://ovz.yongpay.top

[Q49] 更新单行
来源：http://bsr.ywan-chungtsiang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://igq.gaohongyu789.top

[Q50] 批量更新
来源：http://orn.zhaomingkeji.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zux.yonumen.top

[Q51] 用子查询更新
来源：http://npx.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://myp.fehbvm.com

[Q52] 删除指定行
来源：http://nrk.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://hre.daria6918.cn

[Q53] 按条件删除
来源：http://aam.jinghuilouyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qcc.yvedp.cn

[Q54] 清空表
来源：http://mlr.cashguo.top

TRUNCATE TABLE logs;
来源：http://ifu.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://fdt.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aow.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://dos.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://npv.jinyuanbaomall.cn

[Q57] 行号
来源：http://hxq.jinghuilouyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://udz.tanke756.top

[Q58] 累计求和
来源：http://cel.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ejv.feifeiyinyue.top

[Q59] 分组内累计
来源：http://upk.sweek.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lpy.sweek.top

[Q60] 取上一行 / 下一行
来源：http://uwy.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rom.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dde.52xcode.cn

[Q61] 移动平均
来源：http://rtv.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://izd.daria6918.cn

[Q62] 分组占比
来源：http://vpy.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ivj.chenjidiqi.icu

[Q63] 开启事务
来源：http://jga.pengpengdd.cyou

START TRANSACTION;                -- 或 BEGIN
来源：http://djy.birdmap.top

[Q64] 提交事务
来源：http://brq.andypj.xyz

COMMIT;
来源：http://ngz.ydjk.org.cn

[Q65] 回滚事务
来源：http://whr.yvedp.cn

ROLLBACK;
来源：http://eea.yangfankeji.com

[Q66] 行锁查询
来源：http://syi.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://myj.zhixingplan.top

[Q67] 设置隔离级别
来源：http://jmq.aizwys.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jyf.mhx1999.top

[Q68] 保存点
来源：http://ufc.sufxvd.cn

SAVEPOINT sp1;
来源：http://tnj.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://kha.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://rvg.chenzaomai.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ckx.fehbvm.com

[Q70] 更新统计信息
来源：http://aic.jianghu66.top

ANALYZE TABLE users;
来源：http://hpo.kuanghao11.cn

[Q71] 查看建表语句
来源：http://tvi.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dcz.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://ela.ehwqpu.com

SHOW INDEX FROM users;
来源：http://mau.hfpthk.cn

[Q73] 查看表状态
来源：http://xoc.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://awi.hnxiangtu.top

[Q74] 强制使用索引
来源：http://fle.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zds.kuanghao11.cn

[Q75] 日期格式化
来源：http://qto.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mkl.tarul.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gen.sufxvd.cn

[Q76] 按天统计
来源：http://qqm.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lue.feifeiyinyue.top

[Q77] 时间加减
来源：http://rsw.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://djh.bjfxy.top

[Q78] 当前时间
来源：http://pou.birdmap.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wec.gogol.net.cn

[Q79] 字符串拼接
来源：http://uub.jinghuilouyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bkc.bbcook.cn

[Q80] 字符串截取
来源：http://chc.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dbu.cheryme.top

[Q81] 字符串替换
来源：http://wkr.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zqn.tianlin.xyz

[Q82] 字符长度与字节长度
来源：http://wba.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fdg.chenzaomai.com

[Q83] 大小写转换
来源：http://nul.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yzi.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://wmi.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://kmb.fanxiaobao.xyz

[Q85] 数值取整
来源：http://mmo.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ktk.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://blw.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://voa.uphjek.com

[Q87] JSON 字段做条件
来源：http://qqn.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mks.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://rkb.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mar.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qak.shzxlz.cn

[Q89] 判断表是否存在
来源：http://aaf.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ogb.52xcode.cn

[Q90] 生成序号列
来源：http://vkk.smart0.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xpq.guannengcc.top

================================================================================
来源：http://mdn.yanxiufei.cn

R. Bash 专题
来源：http://gsp.andypj.xyz

================================================================================
来源：http://bwz.hysaishi.cn

[R01] shebang 与严格模式
来源：http://xpx.tian-w.cn

#!/usr/bin/env bash
来源：http://aqx.shanyushiyangtech.top

set -euo pipefail
来源：http://uvz.vqdsnc.cn

[R02] 变量赋值与使用
来源：http://brn.iojbl.cn

name="Tom"; echo "$name"
来源：http://npn.gotoacloud.top

[R03] 只读变量
来源：http://pff.9152youxi.cn

readonly PI=3.14
来源：http://cva.gzhubu.top

[R04] 位置参数
来源：http://oew.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sbh.fengsongda.top

[R05] 参数默认值
来源：http://iuj.chenzaomai.com

name="${1:-default}"
来源：http://anu.ppjwa.cn

[R06] 判断命令是否存在
来源：http://oka.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ekz.sysykeji.top

[R07] if 判断文件
来源：http://mmg.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qca.wangdashe.top

[R08] 数值比较
来源：http://pdx.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://swc.xuetiantiany.cn

[R09] 字符串比较
来源：http://jly.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bxm.yj202588.top

[R10] 正则匹配
来源：http://qiz.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aym.daria6918.cn

[R11] case 多分支
来源：http://ict.jinyuanbaomall.cn

case "$1" in
来源：http://iot.zhixingplan.top

start) echo "启动" ;;
来源：http://ffo.redwolf501.top

stop)  echo "停止" ;;
来源：http://pru.c1oappe.top

*)     echo "未知命令" ;;
来源：http://hwp.jinqigufen.top

esac
来源：http://ide.chenzaomai.com

[R12] for 遍历文件
来源：http://njh.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://vvi.gogol.net.cn

[R13] for 计数循环
来源：http://tkd.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://hhe.nanxuanxn.top

[R14] C 风格 for
来源：http://wje.vqdsnc.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pgc.hnqzz.top

[R15] while 逐行读文件
来源：http://kid.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hoq.0kj1m.cn

[R16] until 等待条件
来源：http://nlm.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tzt.c1oappe.top

[R17] 数组定义与取值
来源：http://ntu.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ccs.yanxiufei.cn

[R18] 遍历数组
来源：http://dgv.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nnc.jinyuanbaomall.cn

[R19] 数组长度
来源：http://yat.cucudq.cn

echo "${#arr[@]}"
来源：http://vah.yongpay.top

[R20] 关联数组（字典）
来源：http://tsy.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ndv.jinqigfzy.top

[R21] 字符串长度
来源：http://msi.gaohongyu789.top

echo "${#s}"
来源：http://lqt.dianchejie.cn

[R22] 截取子串
来源：http://uxr.zhiwuduotai.top

echo "${s:0:5}"
来源：http://soi.jyoumei.cn

[R23] 字符串替换
来源：http://wko.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zhk.hcnkem.com

[R24] 大小写转换
来源：http://dae.jqgufenzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://fjz.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://mue.yanxiufei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vac.smart0.xyz

[R26] 命令替换
来源：http://exm.ydzc1.top

now=$(date +%F); echo "$now"
来源：http://cvj.316326.xyz

[R27] 算术展开
来源：http://xix.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://dlb.gzhubu.top

[R28] 浮点运算
来源：http://ggq.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://ihu.ydjk.org.cn

[R29] 定义函数
来源：http://mom.nwbrower.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nqs.shzxlz.cn

[R30] 函数返回状态码
来源：http://fcs.iojbl.cn

f() { return 0; }; f || echo "失败了"
来源：http://npa.hysaishi.cn

[R31] 局部变量
来源：http://uqg.zhixingplan.top

f() { local x=1; echo "$x"; }
来源：http://idc.guannengcc.top

[R32] 参数个数校验
来源：http://vgl.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ltb.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://jla.fengsongda.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cnt.uphjek.com

[R34] 退出时清理
来源：http://ggi.xuetiantiany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pit.zycfv.cn

[R35] 后台执行并等待
来源：http://akf.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uly.fanxiaobao.xyz

[R36] 并发执行多个任务
来源：http://kfc.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://utl.hfpthk.cn

[R37] 把输出赋给变量
来源：http://cor.svipenyu.cn

files=$(ls -1)
来源：http://ydx.cqqwz.cn

[R38] 管道串联
来源：http://ipb.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://ofo.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://wqv.hesvh.cn

cmd > out.log 2>&1
来源：http://trt.feifeiyinyue.top

[R40] 追加写日志
来源：http://aln.xziqi.cn

echo "log" >> out.log
来源：http://miz.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://pcj.xinyue.icu

cmd >/dev/null 2>&1
来源：http://ifc.9152youxi.cn

[R42] 输入重定向
来源：http://jne.gaohongyu789.top

wc -l < a.txt
来源：http://hzs.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://vyg.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://klt.yangfankeji.com

[R44] 按修改时间查找
来源：http://sfi.tian-w.cn

find . -mtime -7 -type f
来源：http://uby.tian-w.cn

[R45] 批量删除
来源：http://nje.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://qem.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://kus.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oew.sweek.top

[R47] sed 单行替换
来源：http://ubq.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hfy.wangshuangyany.cn

[R48] awk 取指定列
来源：http://aik.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://zze.haohaochexian.top

[R49] awk 带条件
来源：http://xxc.ybcxt.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lcu.xinyue.icu

[R50] awk 求和
来源：http://fta.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://srt.yuanzhike.top

[R51] 排序去重取前几
来源：http://ssh.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jwn.hysaishi.cn

[R52] 统计行数
来源：http://czt.guannengcc.top

wc -l a.txt
来源：http://rvj.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://rvu.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sdi.gogol.net.cn

[R54] 比较两个文件
来源：http://mfo.hysaishi.cn

diff a.txt b.txt
来源：http://osx.vehdjk.com

[R55] 压缩与解压
来源：http://lny.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uca.52xcode.cn

[R56] 远程拷贝
来源：http://nox.hnxiangtu.top

scp file user@host:/path/
来源：http://cmz.tian-w.cn

[R57] 远程执行命令
来源：http://snh.sysykeji.top

ssh user@host 'uptime'
来源：http://brv.zhengqikj.top

[R58] 下载文件
来源：http://hkw.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qfd.jlsjyb.cn

[R59] 发 POST JSON
来源：http://wgz.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zkm.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://cqx.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://svy.gzhubu.top

[R61] 磁盘占用
来源：http://ddp.ydjk.org.cn

df -h;  du -sh *
来源：http://dxe.sysykeji.top

[R62] 找最占空间的文件
来源：http://iwj.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://nru.jlsjyb.cn

[R63] 内存与进程
来源：http://bjp.bbcook.cn

free -h;  ps aux | grep nginx
来源：http://ltc.yj20258888.top

[R64] 结束进程
来源：http://apm.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://yxv.yongpay.top

[R65] 查看端口占用
来源：http://qfc.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ctq.ydzc1.top

[R66] 定时任务
来源：http://moi.chenzaomai.com

crontab -e;  crontab -l
来源：http://miw.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://vva.xylfe.cn

openssl rand -hex 16
来源：http://kcf.jianghu66.top

[R68] 计算文件校验值
来源：http://ukb.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dlz.fehbvm.com

[R69] 生成随机密码
来源：http://bjd.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://ysm.jqgfzy.top

[R70] 时间戳与互转
来源：http://cby.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://gyl.dianchejie.cn

[R71] 日期格式化
来源：http://aep.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fge.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://vjf.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://oyd.hnqzz.top

[R73] 分割大日志
来源：http://mhf.jiagoushi.top

split -l 1000 big.log part_
来源：http://rik.yonumen.top

[R74] 批量重命名
来源：http://fte.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eth.sweek.top

[R75] 导出环境变量
来源：http://klt.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://qop.yvedp.cn

[R76] 使用临时文件
来源：http://cch.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://suo.yj202588.top

[R77] 读取用户输入
来源：http://wky.yangfankeji.com

read -rp "请输入: " ans
来源：http://nzd.hysaishi.cn

[R78] 交互式菜单
来源：http://mea.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kxb.zdbjq.cn

[R79] 解析命令行选项
来源：http://jsv.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mce.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://poc.haohaochexian.top

time ./run.sh
来源：http://oxu.jinqigufen.top

================================================================================
来源：http://kvf.ppjwa.cn

S. C / C++ 专题
来源：http://trs.xinyue.icu

================================================================================
来源：http://lfo.gaohongyu789.top

[S01] C：Hello World
来源：http://oxu.sxryk.cn

#include <stdio.h>
来源：http://hkk.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://fag.ybcxt.top

[S02] C：变量与格式化输出
来源：http://fqx.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://mfq.jianghu66.top

[S03] C：读入整数
来源：http://loi.hnqzz.top

int x; scanf("%d", &x);
来源：http://nip.jiagoushi.top

[S04] C：字符串复制
来源：http://gef.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://zas.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://gyw.yfazqb.com

strlen(s)
来源：http://adt.pycfn.com

[S06] C：字符串比较
来源：http://slr.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://pry.yj202588.top

[S07] C：数组遍历求和
来源：http://hft.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ymn.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://yqb.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ymu.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://hun.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tdy.yvedp.cn

[S10] C：指针与解引用
来源：http://jst.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://map.bjfxy.top

[S11] C：逐行读文件
来源：http://out.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://qlj.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xpk.aibaodan.cn

fclose(f);
来源：http://ypb.hongshengwenyu.top

[S12] C：写文件
来源：http://kod.fktsv.cn


<!-- 参考信息 -->