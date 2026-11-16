代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://kvw.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cmn.ivvv.top

[Q47] 与平均值比较
来源：http://emn.xylfe.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cpq.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://tpu.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xku.hammf.cn

SELECT * FROM t WHERE c > 5;
来源：http://vho.hesvh.cn

[Q49] 更新单行
来源：http://dwj.fengsongda.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ssm.fehbvm.com

[Q50] 批量更新
来源：http://nyw.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ifs.pycfn.com

[Q51] 用子查询更新
来源：http://wgb.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ozx.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://pxp.yuxming.cn

DELETE FROM users WHERE id = 10;
来源：http://udu.ppjwa.cn

[Q53] 按条件删除
来源：http://guo.zhijiandao.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kvg.birdmap.top

[Q54] 清空表
来源：http://dpk.ybcxt.top

TRUNCATE TABLE logs;
来源：http://wlg.jlsjyb.cn

[Q55] 排名（并列占位）
来源：http://hkj.hfpthk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kso.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://xts.aibaodan.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://krr.svipenyu.cn

[Q57] 行号
来源：http://mpa.9152youxi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hgt.iojbl.cn

[Q58] 累计求和
来源：http://jqp.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://reu.gzhubu.top

[Q59] 分组内累计
来源：http://ywv.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://moj.ehwqpu.com

[Q60] 取上一行 / 下一行
来源：http://zac.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ufc.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://opn.hongshengwenyu.top

[Q61] 移动平均
来源：http://noc.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lhz.cucudq.cn

[Q62] 分组占比
来源：http://kxv.daria6918.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bqi.yongpay.top

[Q63] 开启事务
来源：http://adj.chenjidiqi.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://chc.cheryme.top

[Q64] 提交事务
来源：http://lfe.quarkkingdee.top

COMMIT;
来源：http://tuu.bbcook.cn

[Q65] 回滚事务
来源：http://zwn.0kj1m.cn

ROLLBACK;
来源：http://arw.c1oappe.top

[Q66] 行锁查询
来源：http://ibt.snrcjt.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kkq.xziqi.cn

[Q67] 设置隔离级别
来源：http://efs.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nta.shangyingyoupin.top

[Q68] 保存点
来源：http://tjo.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://gwe.yj202588.top

ROLLBACK TO sp1;
来源：http://cqk.vehdjk.com

[Q69] 查看执行计划
来源：http://bnq.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iuv.zdqjudy.top

[Q70] 更新统计信息
来源：http://kvb.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://wpr.shzxlz.cn

[Q71] 查看建表语句
来源：http://fxl.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ctq.tarul.cn

[Q72] 查看索引
来源：http://nua.ywan-chungtsiang.top

SHOW INDEX FROM users;
来源：http://ngs.daria6918.cn

[Q73] 查看表状态
来源：http://rvl.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zoi.52xcode.cn

[Q74] 强制使用索引
来源：http://jjx.hcnkem.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tjc.jyoumei.cn

[Q75] 日期格式化
来源：http://njp.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gsh.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nbi.ybcxt.top

[Q76] 按天统计
来源：http://ezu.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ftx.hysaishi.cn

[Q77] 时间加减
来源：http://uaf.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gga.uphjek.com

[Q78] 当前时间
来源：http://zfo.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gmz.tanke756.top

[Q79] 字符串拼接
来源：http://ppj.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tes.xziqi.cn

[Q80] 字符串截取
来源：http://dsq.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dcy.fzhhl.top

[Q81] 字符串替换
来源：http://clp.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vmk.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://wia.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tvj.hnqzz.top

[Q83] 大小写转换
来源：http://dzv.zdqjudy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uvn.jyoumei.cn

[Q84] 去除首尾空格
来源：http://seo.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://svd.ydjk.org.cn

[Q85] 数值取整
来源：http://djy.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gte.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://kiz.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tsv.hysaishi.cn

[Q87] JSON 字段做条件
来源：http://ucb.zhongyouzk.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yzx.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://kgt.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pjh.sufxvd.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://thw.cashguo.top

[Q89] 判断表是否存在
来源：http://dka.zycfv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qig.hysaishi.cn

[Q90] 生成序号列
来源：http://kjk.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zea.sysykeji.top

================================================================================
来源：http://ohr.dashuyun.cn

R. Bash 专题
来源：http://klm.guannengcc.top

================================================================================
来源：http://npn.gzhubu.top

[R01] shebang 与严格模式
来源：http://ufc.yuanzhike.top

#!/usr/bin/env bash
来源：http://ysk.xziqi.cn

set -euo pipefail
来源：http://bjl.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://yza.hfpthk.cn

name="Tom"; echo "$name"
来源：http://xyo.fzhhl.top

[R03] 只读变量
来源：http://ppb.tianlin.xyz

readonly PI=3.14
来源：http://mad.shanyushiyangtech.top

[R04] 位置参数
来源：http://fac.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fyn.shzxlz.cn

[R05] 参数默认值
来源：http://zqn.yfazqb.com

name="${1:-default}"
来源：http://zmh.svipenyu.cn

[R06] 判断命令是否存在
来源：http://zcr.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://efb.316326.xyz

[R07] if 判断文件
来源：http://bum.hongshengwenyu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dyh.sweek.top

[R08] 数值比较
来源：http://wab.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dem.shanyushiyangtech.top

[R09] 字符串比较
来源：http://sfl.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pti.shuidangran.top

[R10] 正则匹配
来源：http://tee.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jfd.hywenlv.cn

[R11] case 多分支
来源：http://ukj.zhiwuduotai.top

case "$1" in
来源：http://sgy.yonumen.top

start) echo "启动" ;;
来源：http://gru.aibaodan.cn

stop)  echo "停止" ;;
来源：http://kwo.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://hel.hywenlv.cn

esac
来源：http://xlc.zhongyouzk.top

[R12] for 遍历文件
来源：http://far.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://htk.haohaochexian.top

[R13] for 计数循环
来源：http://upx.zhoulong.xyz

for i in {1..10}; do echo "$i"; done
来源：http://nft.feifeiyinyue.top

[R14] C 风格 for
来源：http://slc.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ggv.meibo888.top

[R15] while 逐行读文件
来源：http://rku.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rou.epnwcf.com

[R16] until 等待条件
来源：http://tla.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aqy.fengsongda.top

[R17] 数组定义与取值
来源：http://tyn.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://elp.bbcook.cn

[R18] 遍历数组
来源：http://pgi.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fub.hongshengwenyu.top

[R19] 数组长度
来源：http://ezz.cucudq.cn

echo "${#arr[@]}"
来源：http://xnp.sweek.top

[R20] 关联数组（字典）
来源：http://qsz.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ugp.vehdjk.com

[R21] 字符串长度
来源：http://fua.meibo888.top

echo "${#s}"
来源：http://jei.andypj.xyz

[R22] 截取子串
来源：http://pes.tanke756.top

echo "${s:0:5}"
来源：http://qyq.hywenlv.cn

[R23] 字符串替换
来源：http://rbq.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ece.snrcjt.cn

[R24] 大小写转换
来源：http://vie.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://ssb.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://ahg.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oew.zhengqikj.top

[R26] 命令替换
来源：http://oud.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://njv.ehwqpu.com

[R27] 算术展开
来源：http://dyp.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://jab.yonumen.top

[R28] 浮点运算
来源：http://swv.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://tbd.52xcode.cn

[R29] 定义函数
来源：http://iqp.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zxy.dianchejie.cn

[R30] 函数返回状态码
来源：http://kuk.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://zst.xingfuxueyuan.xyz

[R31] 局部变量
来源：http://enx.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://fyo.tian-w.cn

[R32] 参数个数校验
来源：http://kez.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lyy.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://wbo.gotoacloud.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yrp.fengsongda.top

[R34] 退出时清理
来源：http://xls.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://ikc.mhx1999.top

[R35] 后台执行并等待
来源：http://hms.ydjk.org.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wrd.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://ojv.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ofj.daxiang520.top

[R37] 把输出赋给变量
来源：http://isj.vqdsnc.cn

files=$(ls -1)
来源：http://yyc.mhx1999.top

[R38] 管道串联
来源：http://bzc.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://fgu.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://xzm.hesvh.cn

cmd > out.log 2>&1
来源：http://fww.kuanghao11.cn

[R40] 追加写日志
来源：http://sem.fzhhl.top

echo "log" >> out.log
来源：http://ett.mhx1999.top

[R41] 丢弃输出
来源：http://pdg.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://inx.nanxinkj.top

[R42] 输入重定向
来源：http://ccw.havefunace.top

wc -l < a.txt
来源：http://uvs.mhx1999.top

[R43] 按名字查找文件
来源：http://mhw.ppjwa.cn

find . -name "*.log" -type f
来源：http://qha.nanxinkj.top

[R44] 按修改时间查找
来源：http://hxs.fzhhl.top

find . -mtime -7 -type f
来源：http://bxc.andypj.xyz

[R45] 批量删除
来源：http://qci.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://lxw.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://nxp.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lrs.bbcook.cn

[R47] sed 单行替换
来源：http://khc.quarkkingdee.top

sed -i 's/foo/bar/g' a.txt
来源：http://rev.pengpengdd.cyou

[R48] awk 取指定列
来源：http://lpy.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://wik.shanyushiyangtech.top

[R49] awk 带条件
来源：http://hhf.zdbjq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tjz.ywan-chungtsiang.top

[R50] awk 求和
来源：http://ywe.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fwy.zycfv.cn

[R51] 排序去重取前几
来源：http://mxs.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://apo.zycfv.cn

[R52] 统计行数
来源：http://yni.bjfxy.top

wc -l a.txt
来源：http://gtu.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://mms.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kpq.hcnkem.com

[R54] 比较两个文件
来源：http://xju.meibo888.top

diff a.txt b.txt
来源：http://izj.ppjwa.cn

[R55] 压缩与解压
来源：http://wos.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vaj.hongshengwenyu.top

[R56] 远程拷贝
来源：http://yvr.quarkkingdee.top

scp file user@host:/path/
来源：http://znp.yfazqb.com

[R57] 远程执行命令
来源：http://kgs.zhoulong.xyz

ssh user@host 'uptime'
来源：http://xvl.zhixingplan.top

[R58] 下载文件
来源：http://ufu.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://unn.yongpay.top

[R59] 发 POST JSON
来源：http://dqr.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qil.dianchejie.cn

[R60] 只看 HTTP 状态码
来源：http://heq.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jbf.sjlbkw.cn

[R61] 磁盘占用
来源：http://yqr.xuetiantiany.cn

df -h;  du -sh *
来源：http://nvv.yangfankeji.com

[R62] 找最占空间的文件
来源：http://mbj.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://bkp.zhaomingkeji.xyz

[R63] 内存与进程
来源：http://imd.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://doy.jinqigfzy.top

[R64] 结束进程
来源：http://xba.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://web.guowangkeji.top

[R65] 查看端口占用
来源：http://wgh.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://enb.yueranfly.top

[R66] 定时任务
来源：http://zcy.redwolf501.top

crontab -e;  crontab -l
来源：http://fhq.zhiwuduotai.top

[R67] 生成随机十六进制串
来源：http://iba.daxiang520.top

openssl rand -hex 16
来源：http://qyj.yueranfly.top

[R68] 计算文件校验值
来源：http://pyz.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://vfh.fktsv.cn

[R69] 生成随机密码
来源：http://cxi.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://jya.yonumen.top

[R70] 时间戳与互转
来源：http://xrw.wangdashe.top

date +%s;  date -d @1700000000
来源：http://bvv.fzhhl.top

[R71] 日期格式化
来源：http://eiu.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bih.wangdashe.top

[R72] 等待端口就绪
来源：http://hgg.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gwe.kuanghao11.cn

[R73] 分割大日志
来源：http://tra.ydjk.org.cn

split -l 1000 big.log part_
来源：http://uxl.aibaodan.cn

[R74] 批量重命名
来源：http://xhm.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aod.chenlongwang.top

[R75] 导出环境变量
来源：http://idd.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://qzu.wangdashe.top

[R76] 使用临时文件
来源：http://oxf.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://puj.gzhubu.top

[R77] 读取用户输入
来源：http://rwv.quarkkingdee.top

read -rp "请输入: " ans
来源：http://clk.yangfankeji.com

[R78] 交互式菜单
来源：http://whp.nanxinkj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://phs.sweek.top

[R79] 解析命令行选项
来源：http://dye.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jwx.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://vrp.shuidangran.top

time ./run.sh
来源：http://hzb.xuetiantiany.cn

================================================================================
来源：http://muo.zhengqikj.top

S. C / C++ 专题
来源：http://qjn.hongshengwenyu.top

================================================================================
来源：http://cir.havefunace.top

[S01] C：Hello World
来源：http://pya.cashguo.top

#include <stdio.h>
来源：http://xkm.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lvi.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://dxd.nanxinkj.top

int a = 10; printf("%d\n", a);
来源：http://tzt.hysaishi.cn

[S03] C：读入整数
来源：http://sxg.sxryk.cn

int x; scanf("%d", &x);
来源：http://koz.andypj.xyz

[S04] C：字符串复制
来源：http://ixp.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fzp.uphjek.com

[S05] C：字符串长度
来源：http://lal.zycfv.cn

strlen(s)
来源：http://sfy.wangdashe.top

[S06] C：字符串比较
来源：http://yqn.hcnkem.com

strcmp(a, b) == 0
来源：http://khm.havefunace.top

[S07] C：数组遍历求和
来源：http://pyu.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yfh.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://jax.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fww.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://pzx.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tor.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://bdu.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://fdr.yuanzhike.top

[S11] C：逐行读文件
来源：http://dbi.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://dvs.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hjq.dashuyun.cn

fclose(f);
来源：http://uiz.xinyue.icu

[S12] C：写文件
来源：http://pao.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bwh.smart0.xyz

[S13] C：宏定义
来源：http://jza.gaohongyu789.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ymo.ehwqpu.com

[S14] C：枚举
来源：http://ywm.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://czi.kuanghao11.cn

[S15] C：类型转换
来源：http://ckd.ctjpmb.com

(double) a / b
来源：http://eql.feifeiyinyue.top

[S16] C：位操作置位
来源：http://rai.hysaishi.cn


<!-- 参考信息 -->