代发 wailian999

[Q48] CTE 公用表表达式
来源：http://cix.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xwc.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://rcr.andypj.xyz

[Q49] 更新单行
来源：http://mmj.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://azt.birdmap.top

[Q50] 批量更新
来源：http://mfj.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://khp.hnqzz.top

[Q51] 用子查询更新
来源：http://irn.kuanghao11.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zgm.hesvh.cn

[Q52] 删除指定行
来源：http://adi.dashuyun.cn

DELETE FROM users WHERE id = 10;
来源：http://tij.fzhhl.top

[Q53] 按条件删除
来源：http://kem.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hod.ywan-chungtsiang.top

[Q54] 清空表
来源：http://cel.xuetiantiany.cn

TRUNCATE TABLE logs;
来源：http://rbs.shanyushiyangkeji.top

[Q55] 排名（并列占位）
来源：http://ldy.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vct.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://pbn.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qlt.hongshengwenyu.top

[Q57] 行号
来源：http://dst.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ecg.chenlongwang.top

[Q58] 累计求和
来源：http://swn.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jnz.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://rjs.meibo888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://thh.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://yvz.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uey.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nsu.zhixingplan.top

[Q61] 移动平均
来源：http://fmr.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yqa.sweek.top

[Q62] 分组占比
来源：http://cbv.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ggi.sweek.top

[Q63] 开启事务
来源：http://iej.yuanzhike.top

START TRANSACTION;                -- 或 BEGIN
来源：http://alx.redwolf501.top

[Q64] 提交事务
来源：http://nsh.ywan-chungtsiang.top

COMMIT;
来源：http://xfh.cdnleiting.top

[Q65] 回滚事务
来源：http://iwt.sjlbkw.cn

ROLLBACK;
来源：http://dfp.fehbvm.com

[Q66] 行锁查询
来源：http://xzn.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ycm.hammf.cn

[Q67] 设置隔离级别
来源：http://xgw.9152youxi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xyr.ybcxt.top

[Q68] 保存点
来源：http://pum.yvedp.cn

SAVEPOINT sp1;
来源：http://smb.0kj1m.cn

ROLLBACK TO sp1;
来源：http://edd.iojbl.cn

[Q69] 查看执行计划
来源：http://vzt.feifeiyinyue.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pte.ivvv.top

[Q70] 更新统计信息
来源：http://yud.nanxinkj.top

ANALYZE TABLE users;
来源：http://whq.hysaishi.cn

[Q71] 查看建表语句
来源：http://gad.shanyushiyangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sur.xinyue.icu

[Q72] 查看索引
来源：http://whm.meibo888.top

SHOW INDEX FROM users;
来源：http://kum.cucudq.cn

[Q73] 查看表状态
来源：http://mfx.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://plj.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://qzc.zhengqikj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yxo.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://loq.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tcg.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kby.ybcxt.top

[Q76] 按天统计
来源：http://jzl.cqqwz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aou.svipenyu.cn

[Q77] 时间加减
来源：http://qnw.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ran.yuanzhike.top

[Q78] 当前时间
来源：http://yar.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qyf.cashguo.top

[Q79] 字符串拼接
来源：http://rbk.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ypv.zhiwuduotai.top

[Q80] 字符串截取
来源：http://cxm.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iin.nanxuanxn.top

[Q81] 字符串替换
来源：http://ecx.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tmy.tarul.cn

[Q82] 字符长度与字节长度
来源：http://unv.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rma.zdbjq.cn

[Q83] 大小写转换
来源：http://woc.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nvv.aibaodan.cn

[Q84] 去除首尾空格
来源：http://lsj.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://wwv.jinghuilouyu.cn

[Q85] 数值取整
来源：http://wji.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kuq.shanyushiyangkeji.top

[Q86] 读取 JSON 字段
来源：http://ema.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bdf.fengsongda.top

[Q87] JSON 字段做条件
来源：http://avq.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://agz.xingfuxueyuan.xyz

[Q88] 行转列（条件聚合）
来源：http://kxu.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pll.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://czk.tanke756.top

[Q89] 判断表是否存在
来源：http://iip.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yhx.quarkkingdee.top

[Q90] 生成序号列
来源：http://ykx.cdnleiting.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://okp.jqgufenzy.top

================================================================================
来源：http://knm.pengpengdd.cyou

R. Bash 专题
来源：http://nda.xinyue.icu

================================================================================
来源：http://wvv.aizwys.cn

[R01] shebang 与严格模式
来源：http://ktq.52xcode.cn

#!/usr/bin/env bash
来源：http://wka.nwbrower.top

set -euo pipefail
来源：http://kdj.cucudq.cn

[R02] 变量赋值与使用
来源：http://bdi.kuanghao11.cn

name="Tom"; echo "$name"
来源：http://soa.hywenlv.cn

[R03] 只读变量
来源：http://kcd.pycfn.com

readonly PI=3.14
来源：http://jxu.yuxming.cn

[R04] 位置参数
来源：http://jih.hongshengwenyu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oge.nanxinkj.top

[R05] 参数默认值
来源：http://lfl.yvedp.cn

name="${1:-default}"
来源：http://mnb.yonumen.top

[R06] 判断命令是否存在
来源：http://ujy.pengpengdd.cyou

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lbp.shzxlz.cn

[R07] if 判断文件
来源：http://qim.hnqzz.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://opf.dashuyun.cn

[R08] 数值比较
来源：http://dyf.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://eaz.chenjidiqi.icu

[R09] 字符串比较
来源：http://ryh.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wad.sweek.top

[R10] 正则匹配
来源：http://djq.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://znn.wangshuangyany.cn

[R11] case 多分支
来源：http://ddb.jyoumei.cn

case "$1" in
来源：http://tbi.fanxiaobao.xyz

start) echo "启动" ;;
来源：http://ebr.vqdsnc.cn

stop)  echo "停止" ;;
来源：http://tww.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://qfq.tianlin.xyz

esac
来源：http://klq.epnwcf.com

[R12] for 遍历文件
来源：http://tid.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://ixr.chenjidiqi.icu

[R13] for 计数循环
来源：http://ufr.ydzc1.top

for i in {1..10}; do echo "$i"; done
来源：http://vjt.xziqi.cn

[R14] C 风格 for
来源：http://xen.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mbx.yongpay.top

[R15] while 逐行读文件
来源：http://fmi.316326.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ukv.kuanghao11.cn

[R16] until 等待条件
来源：http://fbo.hysaishi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xwa.yuanzhike.top

[R17] 数组定义与取值
来源：http://wpo.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://bun.nanxuanxn.top

[R18] 遍历数组
来源：http://jfs.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mie.ppjwa.cn

[R19] 数组长度
来源：http://hcd.sjlbkw.cn

echo "${#arr[@]}"
来源：http://ubn.hesvh.cn

[R20] 关联数组（字典）
来源：http://nqd.ywan-chungtsiang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rav.cashguo.top

[R21] 字符串长度
来源：http://slj.shzxlz.cn

echo "${#s}"
来源：http://pbf.xinyue.icu

[R22] 截取子串
来源：http://mux.aizwys.cn

echo "${s:0:5}"
来源：http://fiq.zhijiandao.cn

[R23] 字符串替换
来源：http://rgl.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zal.sufxvd.cn

[R24] 大小写转换
来源：http://igt.dianchejie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sjl.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://vnv.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jbn.jinqigfzy.top

[R26] 命令替换
来源：http://zly.tanke756.top

now=$(date +%F); echo "$now"
来源：http://eqi.bjfxy.top

[R27] 算术展开
来源：http://udi.hfpthk.cn

echo $((1 + 2 * 3))
来源：http://viz.zhengqikj.top

[R28] 浮点运算
来源：http://cqi.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://yma.zhaomingkeji.xyz

[R29] 定义函数
来源：http://hhl.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://djl.gogol.net.cn

[R30] 函数返回状态码
来源：http://iln.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://cie.ppjwa.cn

[R31] 局部变量
来源：http://cjq.sysykeji.top

f() { local x=1; echo "$x"; }
来源：http://obb.cucudq.cn

[R32] 参数个数校验
来源：http://odn.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nac.xuanzx.com

[R33] 捕获错误并提示行号
来源：http://akv.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://coh.xuetiantiany.cn

[R34] 退出时清理
来源：http://bzl.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://lsb.gogol.net.cn

[R35] 后台执行并等待
来源：http://smc.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://sbt.nanxinkj.top

[R36] 并发执行多个任务
来源：http://spa.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://guh.shzxlz.cn

[R37] 把输出赋给变量
来源：http://ull.jinghuilouyu.cn

files=$(ls -1)
来源：http://tbt.chenzaomai.com

[R38] 管道串联
来源：http://lpa.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://ylq.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://qmb.birdmap.top

cmd > out.log 2>&1
来源：http://qqw.zdbjq.cn

[R40] 追加写日志
来源：http://gwq.hongshengwenyu.top

echo "log" >> out.log
来源：http://ohw.hywenlv.cn

[R41] 丢弃输出
来源：http://anq.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://efk.guannengcc.top

[R42] 输入重定向
来源：http://klv.ydzc1.top

wc -l < a.txt
来源：http://wby.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://ahf.yfazqb.com

find . -name "*.log" -type f
来源：http://vjw.bjfxy.top

[R44] 按修改时间查找
来源：http://fsu.vqdsnc.cn

find . -mtime -7 -type f
来源：http://rle.havefunace.top

[R45] 批量删除
来源：http://sie.xuanzx.com

find . -name "*.tmp" -delete
来源：http://bzq.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://dgc.fanxiaobao.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://krm.hfpthk.cn

[R47] sed 单行替换
来源：http://yfm.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://jwx.bbcook.cn

[R48] awk 取指定列
来源：http://dgc.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://gkz.yfazqb.com

[R49] awk 带条件
来源：http://sdq.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yqm.jiagoushi.top

[R50] awk 求和
来源：http://gin.shangyingyoupin.top

awk '{s += $2} END {print s}' a.txt
来源：http://usm.iojbl.cn

[R51] 排序去重取前几
来源：http://wpd.gotoacloud.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lss.shuidangran.top

[R52] 统计行数
来源：http://lvk.yuxming.cn

wc -l a.txt
来源：http://lgj.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://xvt.sufxvd.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bux.ehwqpu.com

[R54] 比较两个文件
来源：http://ysr.tarul.cn

diff a.txt b.txt
来源：http://uyf.0kj1m.cn

[R55] 压缩与解压
来源：http://gri.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jrw.gzhubu.top

[R56] 远程拷贝
来源：http://zcl.hnxiangtu.top

scp file user@host:/path/
来源：http://qzu.xingfuxueyuan.xyz

[R57] 远程执行命令
来源：http://cro.jyoumei.cn

ssh user@host 'uptime'
来源：http://zyt.nanxuanxn.top

[R58] 下载文件
来源：http://nhm.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://are.sysykeji.top

[R59] 发 POST JSON
来源：http://jwk.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ujk.ydjk.org.cn

[R60] 只看 HTTP 状态码
来源：http://hzx.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cbx.daxiang520.top

[R61] 磁盘占用
来源：http://dhu.yj202588.top

df -h;  du -sh *
来源：http://snu.hesvh.cn

[R62] 找最占空间的文件
来源：http://oqw.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://waj.gaohongyu789.top

[R63] 内存与进程
来源：http://wpn.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://sog.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://ewu.daxiang520.top

kill -9 $(pgrep -f app.py)
来源：http://gtp.zhiwuduotai.top

[R65] 查看端口占用
来源：http://son.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bgf.zhaomingkeji.xyz

[R66] 定时任务
来源：http://adv.yj20258888.top

crontab -e;  crontab -l
来源：http://jhz.ybcxt.top

[R67] 生成随机十六进制串
来源：http://yhs.hongshengwenyu.top

openssl rand -hex 16
来源：http://qzp.jqgfzy.top

[R68] 计算文件校验值
来源：http://bxp.tanke756.top

sha256sum a.txt;  md5sum a.txt
来源：http://tdy.tanke756.top

[R69] 生成随机密码
来源：http://rfo.jinqigfzy.top

head -c 16 /dev/urandom | base64
来源：http://mbh.ybcxt.top

[R70] 时间戳与互转
来源：http://mpx.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://cgb.cqqwz.cn

[R71] 日期格式化
来源：http://ssm.yj202588.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://aup.zhongyouzk.top

[R72] 等待端口就绪
来源：http://fyq.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pqd.mhx1999.top

[R73] 分割大日志
来源：http://cvw.vehdjk.com

split -l 1000 big.log part_
来源：http://pgh.zhixingplan.top

[R74] 批量重命名
来源：http://pym.xuanzx.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ctr.jyoumei.cn

[R75] 导出环境变量
来源：http://ody.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://nnq.ydjk.org.cn

[R76] 使用临时文件
来源：http://wfl.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ync.uphjek.com

[R77] 读取用户输入
来源：http://nbu.zhixingplan.top

read -rp "请输入: " ans
来源：http://knj.svipenyu.cn

[R78] 交互式菜单
来源：http://vcf.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://rja.dianchejie.cn

[R79] 解析命令行选项
来源：http://pjo.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vmx.yongpay.top

[R80] 查看脚本执行耗时
来源：http://hst.tanke756.top

time ./run.sh
来源：http://qrj.316326.xyz

================================================================================
来源：http://zhs.iojbl.cn

S. C / C++ 专题
来源：http://snj.cashguo.top

================================================================================
来源：http://nbb.pengpengdd.cyou

[S01] C：Hello World
来源：http://bls.vqdsnc.cn

#include <stdio.h>
来源：http://lte.meibo888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kai.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://elu.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://tfa.vqdsnc.cn

[S03] C：读入整数
来源：http://wwz.yj20258.top

int x; scanf("%d", &x);
来源：http://kwv.hywenlv.cn

[S04] C：字符串复制
来源：http://jlc.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rur.zhoulong.xyz

[S05] C：字符串长度
来源：http://gep.hysaishi.cn

strlen(s)
来源：http://ico.ybcxt.top

[S06] C：字符串比较
来源：http://udq.ydjk.org.cn

strcmp(a, b) == 0
来源：http://mej.sweek.top

[S07] C：数组遍历求和
来源：http://nle.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ycw.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://rjo.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://puz.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://qwg.cashguo.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ekj.sxryk.cn

[S10] C：指针与解引用
来源：http://baw.yvedp.cn

int *p = &a;  *p = 5;
来源：http://jrl.tianlin.xyz

[S11] C：逐行读文件
来源：http://lwi.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://xhj.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://umo.cheryme.top

fclose(f);
来源：http://tmh.zhengqikj.top

[S12] C：写文件
来源：http://iko.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yva.cdnleiting.top

[S13] C：宏定义
来源：http://gwx.svipenyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bmb.zhijiandao.cn

[S14] C：枚举
来源：http://krb.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://fya.hnqzz.top

[S15] C：类型转换
来源：http://jxf.316326.xyz

(double) a / b
来源：http://hql.hnxiangtu.top

[S16] C：位操作置位
来源：http://uos.cucudq.cn

x |= (1 << 3);
来源：http://ptt.tian-w.cn

[S17] C：安全拼接字符串
来源：http://hbi.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ipm.ehwqpu.com

[S18] C：命令行参数
来源：http://xwi.uphjek.com


<!-- 参考信息 -->