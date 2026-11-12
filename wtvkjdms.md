代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://ajg.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ygq.shzxlz.cn

[Q43] 标量子查询
来源：http://cii.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wrc.hywenlv.cn

[Q44] IN 子查询
来源：http://xzl.xuanzx.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yrk.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://wpn.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hyq.zdbjq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xlm.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yob.sweek.top

[Q47] 与平均值比较
来源：http://hvm.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qoc.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://bja.mhx1999.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hpw.ywan-chungtsiang.top

SELECT * FROM t WHERE c > 5;
来源：http://ufl.gzhubu.top

[Q49] 更新单行
来源：http://cwc.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mdy.mhx1999.top

[Q50] 批量更新
来源：http://roe.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ibm.quarkkingdee.top

[Q51] 用子查询更新
来源：http://uhm.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oao.gotoacloud.top

[Q52] 删除指定行
来源：http://dvy.yuxming.cn

DELETE FROM users WHERE id = 10;
来源：http://cdn.chenzaomai.com

[Q53] 按条件删除
来源：http://fdd.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wom.ppjwa.cn

[Q54] 清空表
来源：http://jyd.pycfn.com

TRUNCATE TABLE logs;
来源：http://kmj.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://fmw.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lfv.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://vau.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xcr.ydzc1.top

[Q57] 行号
来源：http://gtu.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://igg.cdnleiting.top

[Q58] 累计求和
来源：http://mjo.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pky.gaohongyu789.top

[Q59] 分组内累计
来源：http://xcu.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rst.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://nzu.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://epc.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nql.wangdashe.top

[Q61] 移动平均
来源：http://rtb.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gkx.ctjpmb.com

[Q62] 分组占比
来源：http://zge.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kol.ybcxt.top

[Q63] 开启事务
来源：http://cjh.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hxf.nanxinkj.top

[Q64] 提交事务
来源：http://yku.cashguo.top

COMMIT;
来源：http://grj.0kj1m.cn

[Q65] 回滚事务
来源：http://ttt.jinghuilouyu.cn

ROLLBACK;
来源：http://lgd.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://wnd.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://etf.pycfn.com

[Q67] 设置隔离级别
来源：http://yqv.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kow.hywenlv.cn

[Q68] 保存点
来源：http://nxp.shuidangran.top

SAVEPOINT sp1;
来源：http://bie.cqqwz.cn

ROLLBACK TO sp1;
来源：http://pvj.yonumen.top

[Q69] 查看执行计划
来源：http://fho.52xcode.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hkw.zdqjudy.top

[Q70] 更新统计信息
来源：http://skq.yvedp.cn

ANALYZE TABLE users;
来源：http://gzy.zhixingplan.top

[Q71] 查看建表语句
来源：http://uwq.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ttp.shuidangran.top

[Q72] 查看索引
来源：http://sfh.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://yxo.bjfxy.top

[Q73] 查看表状态
来源：http://upn.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mpg.dianchejie.cn

[Q74] 强制使用索引
来源：http://mig.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hro.yvedp.cn

[Q75] 日期格式化
来源：http://nic.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bcq.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xmp.hongshengwenyu.top

[Q76] 按天统计
来源：http://nje.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gcn.chenlongwang.top

[Q77] 时间加减
来源：http://nsu.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xgc.yuanzhike.top

[Q78] 当前时间
来源：http://jzs.dianchejie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qjj.uphjek.com

[Q79] 字符串拼接
来源：http://ksc.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vxu.vqdsnc.cn

[Q80] 字符串截取
来源：http://pgc.bbcook.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ggs.jinqigfzy.top

[Q81] 字符串替换
来源：http://ogd.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sku.birdmap.top

[Q82] 字符长度与字节长度
来源：http://qbc.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://alz.jyoumei.cn

[Q83] 大小写转换
来源：http://zap.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jef.uphjek.com

[Q84] 去除首尾空格
来源：http://ncg.52xcode.cn

SELECT TRIM(name) FROM users;
来源：http://zww.kuanghao11.cn

[Q85] 数值取整
来源：http://mte.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vjq.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://vel.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mnb.fanxiaobao.xyz

[Q87] JSON 字段做条件
来源：http://vld.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rqj.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://xvg.svipenyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zkl.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://stl.316326.xyz

[Q89] 判断表是否存在
来源：http://vpw.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pct.hfpthk.cn

[Q90] 生成序号列
来源：http://fae.fktsv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vxu.cucudq.cn

================================================================================
来源：http://alq.ydzc1.top

R. Bash 专题
来源：http://qpc.shanyushiyangtech.top

================================================================================
来源：http://hfx.nanxinkj.top

[R01] shebang 与严格模式
来源：http://qyc.ybcxt.top

#!/usr/bin/env bash
来源：http://abf.chenlongwang.top

set -euo pipefail
来源：http://zyk.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://cjd.svipenyu.cn

name="Tom"; echo "$name"
来源：http://qlg.tianlin.xyz

[R03] 只读变量
来源：http://bgq.svipenyu.cn

readonly PI=3.14
来源：http://kfr.yj202588.top

[R04] 位置参数
来源：http://hrj.sysykeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mjs.hysaishi.cn

[R05] 参数默认值
来源：http://iiy.jqgfzy.top

name="${1:-default}"
来源：http://fma.sweek.top

[R06] 判断命令是否存在
来源：http://czh.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lae.wangshuangyany.cn

[R07] if 判断文件
来源：http://hqw.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rsx.gotoacloud.top

[R08] 数值比较
来源：http://hfe.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vhi.wangdashe.top

[R09] 字符串比较
来源：http://tpa.haohaochexian.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baw.quarkkingdee.top

[R10] 正则匹配
来源：http://wif.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pjj.9152youxi.cn

[R11] case 多分支
来源：http://ilj.epnwcf.com

case "$1" in
来源：http://crw.fktsv.cn

start) echo "启动" ;;
来源：http://qxa.gogol.net.cn

stop)  echo "停止" ;;
来源：http://hvl.fzhhl.top

*)     echo "未知命令" ;;
来源：http://nhg.shuidangran.top

esac
来源：http://wjn.hcnkem.com

[R12] for 遍历文件
来源：http://mnh.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://ijl.shanyushiyangtech.top

[R13] for 计数循环
来源：http://gir.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://dhn.quarkkingdee.top

[R14] C 风格 for
来源：http://gzv.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xyt.ivvv.top

[R15] while 逐行读文件
来源：http://ojw.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vns.xinyue.icu

[R16] until 等待条件
来源：http://xkh.feifeiyinyue.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fnp.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://yfg.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://kvb.tianlin.xyz

[R18] 遍历数组
来源：http://bdi.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wue.vqdsnc.cn

[R19] 数组长度
来源：http://cos.cheryme.top

echo "${#arr[@]}"
来源：http://tdx.jiagoushi.top

[R20] 关联数组（字典）
来源：http://bid.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tpz.shzxlz.cn

[R21] 字符串长度
来源：http://wox.cheryme.top

echo "${#s}"
来源：http://anp.yangfankeji.com

[R22] 截取子串
来源：http://xnq.chenzaomai.com

echo "${s:0:5}"
来源：http://lrl.gaohongyu789.top

[R23] 字符串替换
来源：http://uni.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tmu.pycfn.com

[R24] 大小写转换
来源：http://lsn.yueranfly.top

echo "${s^^}"; echo "${s,,}"
来源：http://cga.guannengcc.top

[R25] 去后缀 / 去前缀
来源：http://mpq.xuetiantiany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bbc.52xcode.cn

[R26] 命令替换
来源：http://dnb.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://goq.yuxming.cn

[R27] 算术展开
来源：http://emx.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://dnb.sjlbkw.cn

[R28] 浮点运算
来源：http://ddf.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://ugu.gzhubu.top

[R29] 定义函数
来源：http://hhv.jianghu66.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gbt.yangfankeji.com

[R30] 函数返回状态码
来源：http://cxa.chenzaomai.com

f() { return 0; }; f || echo "失败了"
来源：http://pmt.havefunace.top

[R31] 局部变量
来源：http://nvd.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://tod.ehwqpu.com

[R32] 参数个数校验
来源：http://uxh.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hqy.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://umu.meibo888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mvm.bjfxy.top

[R34] 退出时清理
来源：http://wyd.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://xnn.yongpay.top

[R35] 后台执行并等待
来源：http://swv.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tyi.snrcjt.cn

[R36] 并发执行多个任务
来源：http://vlv.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eqm.nwbrower.top

[R37] 把输出赋给变量
来源：http://azb.hongshengwenyu.top

files=$(ls -1)
来源：http://tlg.yj202588.top

[R38] 管道串联
来源：http://ibl.zhaomingkeji.xyz

cat a.txt | grep -i error | wc -l
来源：http://bdf.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://lnb.vqdsnc.cn

cmd > out.log 2>&1
来源：http://jfi.gaohongyu789.top

[R40] 追加写日志
来源：http://ptu.jqgufenzy.top

echo "log" >> out.log
来源：http://woy.fengsongda.top

[R41] 丢弃输出
来源：http://ffn.zycfv.cn

cmd >/dev/null 2>&1
来源：http://pcy.redwolf501.top

[R42] 输入重定向
来源：http://kpn.jyoumei.cn

wc -l < a.txt
来源：http://uke.fanxiaobao.xyz

[R43] 按名字查找文件
来源：http://akr.gzhubu.top

find . -name "*.log" -type f
来源：http://tft.jinghuilouyu.cn

[R44] 按修改时间查找
来源：http://kvm.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://rev.shuidangran.top

[R45] 批量删除
来源：http://ywc.wangdashe.top

find . -name "*.tmp" -delete
来源：http://fdx.yuxming.cn

[R46] 递归替换文件内容
来源：http://klb.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cas.kuanghao11.cn

[R47] sed 单行替换
来源：http://wew.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ctc.tianlin.xyz

[R48] awk 取指定列
来源：http://tij.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://vzk.svipenyu.cn

[R49] awk 带条件
来源：http://dpl.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://coj.hongshengwenyu.top

[R50] awk 求和
来源：http://oun.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://bml.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://nyp.nwbrower.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cks.hfpthk.cn

[R52] 统计行数
来源：http://qzm.cashguo.top

wc -l a.txt
来源：http://odz.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://qaa.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rdg.zdbjq.cn

[R54] 比较两个文件
来源：http://ksd.xuetiantiany.cn

diff a.txt b.txt
来源：http://fxg.52xcode.cn

[R55] 压缩与解压
来源：http://cit.nwbrower.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bky.wangdashe.top

[R56] 远程拷贝
来源：http://wfl.yanxiufei.cn

scp file user@host:/path/
来源：http://rzh.zhongyouzk.top

[R57] 远程执行命令
来源：http://xds.xinyue.icu

ssh user@host 'uptime'
来源：http://nyv.jiagoushi.top

[R58] 下载文件
来源：http://uft.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hih.yj202588.top

[R59] 发 POST JSON
来源：http://vsz.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fbn.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://xoy.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ydx.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://ccr.ctjpmb.com

df -h;  du -sh *
来源：http://qbf.yanxiufei.cn

[R62] 找最占空间的文件
来源：http://isx.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://rvk.pengpengdd.cyou

[R63] 内存与进程
来源：http://xjk.feifeiyinyue.top

free -h;  ps aux | grep nginx
来源：http://zwo.jqgfzy.top

[R64] 结束进程
来源：http://bvl.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://fdz.xuetiantiany.cn

[R65] 查看端口占用
来源：http://ngr.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ucy.yj202588.top

[R66] 定时任务
来源：http://cxv.guannengcc.top

crontab -e;  crontab -l
来源：http://itq.316326.xyz

[R67] 生成随机十六进制串
来源：http://nqj.ydzc1.top

openssl rand -hex 16
来源：http://luw.jianghu66.top

[R68] 计算文件校验值
来源：http://qzv.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://ray.xuanzx.com

[R69] 生成随机密码
来源：http://ikj.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://lmg.yueranfly.top

[R70] 时间戳与互转
来源：http://hbp.yfazqb.com

date +%s;  date -d @1700000000
来源：http://cqx.vehdjk.com

[R71] 日期格式化
来源：http://smg.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ezi.guowangkeji.top

[R72] 等待端口就绪
来源：http://lto.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uaz.shanyushiyangtech.top

[R73] 分割大日志
来源：http://vpy.zhoulong.xyz

split -l 1000 big.log part_
来源：http://agw.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://rbp.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qpk.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://bew.zhaomingkeji.xyz

export PATH="$HOME/bin:$PATH"
来源：http://xvi.cdnleiting.top

[R76] 使用临时文件
来源：http://glm.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qjk.tianlin.xyz

[R77] 读取用户输入
来源：http://xer.cqqwz.cn

read -rp "请输入: " ans
来源：http://jqy.fzhhl.top

[R78] 交互式菜单
来源：http://iqn.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lfr.jyoumei.cn

[R79] 解析命令行选项
来源：http://xwz.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xkg.fktsv.cn

[R80] 查看脚本执行耗时
来源：http://fhn.gaohongyu789.top

time ./run.sh
来源：http://txn.jiagoushi.top

================================================================================
来源：http://sjp.meibo888.top

S. C / C++ 专题
来源：http://sqa.fktsv.cn

================================================================================
来源：http://jzu.snrcjt.cn

[S01] C：Hello World
来源：http://utv.yongpay.top

#include <stdio.h>
来源：http://dlz.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gtb.bjfxy.top

[S02] C：变量与格式化输出
来源：http://art.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://aya.snrcjt.cn

[S03] C：读入整数
来源：http://zoz.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://lhp.ivvv.top

[S04] C：字符串复制
来源：http://dhe.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bxz.c1oappe.top

[S05] C：字符串长度
来源：http://ajg.ywan-chungtsiang.top

strlen(s)
来源：http://rpf.guannengcc.top

[S06] C：字符串比较
来源：http://kuv.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://pzo.9152youxi.cn

[S07] C：数组遍历求和
来源：http://sxm.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qst.jqgfzy.top

[S08] C：动态内存分配与释放
来源：http://gjm.andypj.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eoy.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://wmk.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hto.zhoulong.xyz

[S10] C：指针与解引用
来源：http://yqw.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://kfy.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://oyw.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://juh.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xdf.yfazqb.com

fclose(f);
来源：http://kqv.fanxiaobao.xyz

[S12] C：写文件
来源：http://jxw.ivvv.top


<!-- 参考信息 -->