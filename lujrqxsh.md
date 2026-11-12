代发 wailian999

[Q48] CTE 公用表表达式
来源：http://oua.tanke756.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ats.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://lua.sweek.top

[Q49] 更新单行
来源：http://usl.jqgufenzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baj.hywenlv.cn

[Q50] 批量更新
来源：http://wyn.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sfm.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://mja.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yqq.316326.xyz

[Q52] 删除指定行
来源：http://eok.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://akt.guowangkeji.top

[Q53] 按条件删除
来源：http://akz.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hyt.0kj1m.cn

[Q54] 清空表
来源：http://bzd.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://jax.uphjek.com

[Q55] 排名（并列占位）
来源：http://bml.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zhe.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://iml.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uko.tanke756.top

[Q57] 行号
来源：http://vux.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wut.ivvv.top

[Q58] 累计求和
来源：http://xop.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eht.fengsongda.top

[Q59] 分组内累计
来源：http://far.hcnkem.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ypd.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://fuk.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ssn.zhixingplan.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cnl.cashguo.top

[Q61] 移动平均
来源：http://cdf.nanxuanxn.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ysu.gaohongyu789.top

[Q62] 分组占比
来源：http://okp.wangdashe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bzj.vehdjk.com

[Q63] 开启事务
来源：http://qiz.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bam.tianlin.xyz

[Q64] 提交事务
来源：http://agh.jyoumei.cn

COMMIT;
来源：http://yhh.52xcode.cn

[Q65] 回滚事务
来源：http://wxn.hnxiangtu.top

ROLLBACK;
来源：http://dio.cdnleiting.top

[Q66] 行锁查询
来源：http://vlg.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qcb.9152youxi.cn

[Q67] 设置隔离级别
来源：http://whn.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dpf.gaohongyu789.top

[Q68] 保存点
来源：http://cle.uphjek.com

SAVEPOINT sp1;
来源：http://wmc.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://klu.yj20258888.top

[Q69] 查看执行计划
来源：http://wgv.c1oappe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xdf.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://scv.zdqjudy.top

ANALYZE TABLE users;
来源：http://csv.haohaochexian.top

[Q71] 查看建表语句
来源：http://xjf.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rut.meibo888.top

[Q72] 查看索引
来源：http://ovt.vehdjk.com

SHOW INDEX FROM users;
来源：http://cvs.shuidangran.top

[Q73] 查看表状态
来源：http://qkp.yuxming.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gfk.xuetiantiany.cn

[Q74] 强制使用索引
来源：http://uvt.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nuz.jinqigufen.top

[Q75] 日期格式化
来源：http://hal.pengpengdd.cyou

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lzf.yanxiufei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bld.jinqigufen.top

[Q76] 按天统计
来源：http://qgb.xuanzx.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kcm.epnwcf.com

[Q77] 时间加减
来源：http://bii.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xaf.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://toh.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tgx.zhaomingkeji.xyz

[Q79] 字符串拼接
来源：http://pwv.jqgfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zga.jqgufenzy.top

[Q80] 字符串截取
来源：http://ewy.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://maz.shuidangran.top

[Q81] 字符串替换
来源：http://vmz.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wfl.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://ygv.chenjidiqi.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xqq.yueranfly.top

[Q83] 大小写转换
来源：http://nzv.chenjidiqi.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ilz.gogol.net.cn

[Q84] 去除首尾空格
来源：http://fqd.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://ajv.cucudq.cn

[Q85] 数值取整
来源：http://jnb.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mru.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://xnj.ctjpmb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fgn.yj20258888.top

[Q87] JSON 字段做条件
来源：http://pqq.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://omf.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://jzv.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://emy.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://csa.jqgfzy.top

[Q89] 判断表是否存在
来源：http://czw.xuetiantiany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ose.hcnkem.com

[Q90] 生成序号列
来源：http://rhu.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bnz.jlsjyb.cn

================================================================================
来源：http://xds.birdmap.top

R. Bash 专题
来源：http://pxe.quarkkingdee.top

================================================================================
来源：http://grk.jiagoushi.top

[R01] shebang 与严格模式
来源：http://lvj.sjlbkw.cn

#!/usr/bin/env bash
来源：http://yto.vqdsnc.cn

set -euo pipefail
来源：http://jeq.ybcxt.top

[R02] 变量赋值与使用
来源：http://hts.fehbvm.com

name="Tom"; echo "$name"
来源：http://yfj.ctjpmb.com

[R03] 只读变量
来源：http://htw.dashuyun.cn

readonly PI=3.14
来源：http://yue.bbcook.cn

[R04] 位置参数
来源：http://jgk.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://leo.mhx1999.top

[R05] 参数默认值
来源：http://kty.daria6918.cn

name="${1:-default}"
来源：http://lwd.fktsv.cn

[R06] 判断命令是否存在
来源：http://one.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ket.ydjk.org.cn

[R07] if 判断文件
来源：http://voo.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ujk.shanyushiyangkeji.top

[R08] 数值比较
来源：http://jbf.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://osz.wangdashe.top

[R09] 字符串比较
来源：http://ebx.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cej.tanke756.top

[R10] 正则匹配
来源：http://zwp.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://miu.chenzaomai.com

[R11] case 多分支
来源：http://bkb.vqdsnc.cn

case "$1" in
来源：http://bez.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://ymy.redwolf501.top

stop)  echo "停止" ;;
来源：http://dph.andypj.xyz

*)     echo "未知命令" ;;
来源：http://tal.cashguo.top

esac
来源：http://hba.jqgufenzy.top

[R12] for 遍历文件
来源：http://mgf.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://gpm.9152youxi.cn

[R13] for 计数循环
来源：http://vlz.daxiang520.top

for i in {1..10}; do echo "$i"; done
来源：http://ksq.jinqigufen.top

[R14] C 风格 for
来源：http://ofh.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://snx.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://zbj.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cfz.zhoulong.xyz

[R16] until 等待条件
来源：http://hpk.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mfy.jiagoushi.top

[R17] 数组定义与取值
来源：http://xap.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://dvx.jinghuilouyu.cn

[R18] 遍历数组
来源：http://vio.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zeo.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://ewq.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://ufy.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://srl.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gpw.yuanzhike.top

[R21] 字符串长度
来源：http://zyd.gaohongyu789.top

echo "${#s}"
来源：http://sge.hammf.cn

[R22] 截取子串
来源：http://auc.sysykeji.top

echo "${s:0:5}"
来源：http://xrt.fzhhl.top

[R23] 字符串替换
来源：http://xvn.xuanzx.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://axr.yuanzhike.top

[R24] 大小写转换
来源：http://qwo.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://ayb.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://tzw.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://izk.fengsongda.top

[R26] 命令替换
来源：http://din.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://jek.yongpay.top

[R27] 算术展开
来源：http://bfb.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://iwt.shuidangran.top

[R28] 浮点运算
来源：http://vsb.sweek.top

echo "scale=2; 10/3" | bc
来源：http://kgr.cashguo.top

[R29] 定义函数
来源：http://waz.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mil.sufxvd.cn

[R30] 函数返回状态码
来源：http://fsd.gaohongyu789.top

f() { return 0; }; f || echo "失败了"
来源：http://hxe.zhiwuduotai.top

[R31] 局部变量
来源：http://zwu.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://umy.zhixingplan.top

[R32] 参数个数校验
来源：http://pnd.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dlu.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://jgy.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hnu.fanxiaobao.xyz

[R34] 退出时清理
来源：http://ctt.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://gek.redwolf501.top

[R35] 后台执行并等待
来源：http://lxt.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://emq.gzhubu.top

[R36] 并发执行多个任务
来源：http://njw.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mgv.cucudq.cn

[R37] 把输出赋给变量
来源：http://vjp.ybcxt.top

files=$(ls -1)
来源：http://wfo.epnwcf.com

[R38] 管道串联
来源：http://mjw.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://shr.xuanzx.com

[R39] 重定向标准输出与错误
来源：http://zpz.zhengqikj.top

cmd > out.log 2>&1
来源：http://nex.yj202588.top

[R40] 追加写日志
来源：http://wjk.ydzc1.top

echo "log" >> out.log
来源：http://uva.zdqjudy.top

[R41] 丢弃输出
来源：http://jxr.fehbvm.com

cmd >/dev/null 2>&1
来源：http://rtq.wangdashe.top

[R42] 输入重定向
来源：http://tps.wangdashe.top

wc -l < a.txt
来源：http://nbb.havefunace.top

[R43] 按名字查找文件
来源：http://ytt.jlsjyb.cn

find . -name "*.log" -type f
来源：http://cdu.hysaishi.cn

[R44] 按修改时间查找
来源：http://puk.jqgufenzy.top

find . -mtime -7 -type f
来源：http://zws.nanxinkj.top

[R45] 批量删除
来源：http://vri.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://trm.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://yej.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rcl.cashguo.top

[R47] sed 单行替换
来源：http://yfy.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://wsa.cqqwz.cn

[R48] awk 取指定列
来源：http://nmk.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://msn.jqgfzy.top

[R49] awk 带条件
来源：http://ihy.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cth.wangdashe.top

[R50] awk 求和
来源：http://wry.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://kte.aibaodan.cn

[R51] 排序去重取前几
来源：http://ryh.havefunace.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xcb.guannengcc.top

[R52] 统计行数
来源：http://rmz.jiagoushi.top

wc -l a.txt
来源：http://umy.uphjek.com

[R53] 查看文件头与实时尾
来源：http://jyc.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lwj.zhengqikj.top

[R54] 比较两个文件
来源：http://xux.sufxvd.cn

diff a.txt b.txt
来源：http://ckf.aizwys.cn

[R55] 压缩与解压
来源：http://aak.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://phq.guowangkeji.top

[R56] 远程拷贝
来源：http://zaj.wangdashe.top

scp file user@host:/path/
来源：http://gnx.shuidangran.top

[R57] 远程执行命令
来源：http://kgq.iojbl.cn

ssh user@host 'uptime'
来源：http://pbe.vqdsnc.cn

[R58] 下载文件
来源：http://hqu.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hlv.xinyue.icu

[R59] 发 POST JSON
来源：http://vzd.shzxlz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zth.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://gfy.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mtr.yfazqb.com

[R61] 磁盘占用
来源：http://qjj.xziqi.cn

df -h;  du -sh *
来源：http://zjn.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://rmt.yuanzhike.top

du -ah . | sort -rh | head -10
来源：http://sqh.ehwqpu.com

[R63] 内存与进程
来源：http://vpw.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://jxb.xuanzx.com

[R64] 结束进程
来源：http://hcg.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://unh.hfpthk.cn

[R65] 查看端口占用
来源：http://xsy.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hdb.tian-w.cn

[R66] 定时任务
来源：http://zwp.ydzc1.top

crontab -e;  crontab -l
来源：http://lit.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://gbp.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://wrf.pengpengdd.cyou

[R68] 计算文件校验值
来源：http://piu.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gsf.zdbjq.cn

[R69] 生成随机密码
来源：http://ilc.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://hwh.fengsongda.top

[R70] 时间戳与互转
来源：http://rdk.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://xgp.andypj.xyz

[R71] 日期格式化
来源：http://ize.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pmj.fehbvm.com

[R72] 等待端口就绪
来源：http://jsz.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://dxd.hysaishi.cn

[R73] 分割大日志
来源：http://yeb.zycfv.cn

split -l 1000 big.log part_
来源：http://cqa.vehdjk.com

[R74] 批量重命名
来源：http://sgx.tarul.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lms.xziqi.cn

[R75] 导出环境变量
来源：http://jiu.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://bek.sufxvd.cn

[R76] 使用临时文件
来源：http://drr.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://inw.ydzc1.top

[R77] 读取用户输入
来源：http://kaa.zdqjudy.top

read -rp "请输入: " ans
来源：http://pnd.bbcook.cn

[R78] 交互式菜单
来源：http://hlj.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qly.gaohongyu789.top

[R79] 解析命令行选项
来源：http://tdi.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dgm.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://plx.xuanzx.com

time ./run.sh
来源：http://slp.ybcxt.top

================================================================================
来源：http://gob.hesvh.cn

S. C / C++ 专题
来源：http://dsr.hysaishi.cn

================================================================================
来源：http://yso.pycfn.com

[S01] C：Hello World
来源：http://ame.dianchejie.cn

#include <stdio.h>
来源：http://ulb.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dwq.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://twn.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://jtr.wangdashe.top

[S03] C：读入整数
来源：http://wge.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://riw.hesvh.cn

[S04] C：字符串复制
来源：http://mul.shanyushiyangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://iqa.tianlin.xyz

[S05] C：字符串长度
来源：http://vcz.zhoulong.xyz

strlen(s)
来源：http://snt.fengsongda.top

[S06] C：字符串比较
来源：http://hxk.bbcook.cn

strcmp(a, b) == 0
来源：http://xdl.gzhubu.top

[S07] C：数组遍历求和
来源：http://pxl.wangshuangyany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nqy.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://qcf.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qzz.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://euf.dianchejie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xrp.haohaochexian.top

[S10] C：指针与解引用
来源：http://xve.jianghu66.top

int *p = &a;  *p = 5;
来源：http://tiq.meibo888.top

[S11] C：逐行读文件
来源：http://gsn.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://xgy.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://qpz.yongpay.top

fclose(f);
来源：http://tke.tarul.cn

[S12] C：写文件
来源：http://brs.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hwm.jinghuilouyu.cn

[S13] C：宏定义
来源：http://vda.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://los.vqdsnc.cn

[S14] C：枚举
来源：http://zes.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://erm.9152youxi.cn

[S15] C：类型转换
来源：http://gcc.bbcook.cn

(double) a / b
来源：http://boh.iojbl.cn

[S16] C：位操作置位
来源：http://frb.pengpengdd.cyou

x |= (1 << 3);
来源：http://kjf.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://wxs.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ohk.9152youxi.cn

[S18] C：命令行参数
来源：http://igb.sjlbkw.cn


<!-- 参考信息 -->