代发 wailian999

[Q48] CTE 公用表表达式
来源：http://tio.zhaomingkeji.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tsn.316326.xyz

SELECT * FROM t WHERE c > 5;
来源：http://vls.dashuyun.cn

[Q49] 更新单行
来源：http://kdb.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://exn.daria6918.cn

[Q50] 批量更新
来源：http://can.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eoq.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://mdb.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tii.aizwys.cn

[Q52] 删除指定行
来源：http://csf.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://fbm.sxryk.cn

[Q53] 按条件删除
来源：http://awr.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zms.ydjk.org.cn

[Q54] 清空表
来源：http://cek.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://kjo.xinyue.icu

[Q55] 排名（并列占位）
来源：http://bpa.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uow.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://nct.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hzy.hnqzz.top

[Q57] 行号
来源：http://krv.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tpz.xinyue.icu

[Q58] 累计求和
来源：http://nsl.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pcd.zdbjq.cn

[Q59] 分组内累计
来源：http://muu.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jqw.jlsjyb.cn

[Q60] 取上一行 / 下一行
来源：http://rsz.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://egg.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xqh.ctjpmb.com

[Q61] 移动平均
来源：http://lbp.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lgp.ivvv.top

[Q62] 分组占比
来源：http://zju.yj20258888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aqt.dianchejie.cn

[Q63] 开启事务
来源：http://kak.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ekn.fzhhl.top

[Q64] 提交事务
来源：http://ujl.gotoacloud.top

COMMIT;
来源：http://zmd.kuanghao11.cn

[Q65] 回滚事务
来源：http://jbs.yongpay.top

ROLLBACK;
来源：http://dlf.zhijiandao.cn

[Q66] 行锁查询
来源：http://ngk.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xru.zycfv.cn

[Q67] 设置隔离级别
来源：http://ufg.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://okk.redwolf501.top

[Q68] 保存点
来源：http://sqk.smart0.xyz

SAVEPOINT sp1;
来源：http://fou.ehwqpu.com

ROLLBACK TO sp1;
来源：http://abi.0kj1m.cn

[Q69] 查看执行计划
来源：http://mwr.sxryk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jna.sxryk.cn

[Q70] 更新统计信息
来源：http://vyi.cqqwz.cn

ANALYZE TABLE users;
来源：http://lrt.hesvh.cn

[Q71] 查看建表语句
来源：http://kkb.yuxming.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://agu.xinyue.icu

[Q72] 查看索引
来源：http://rhb.nanxuanxn.top

SHOW INDEX FROM users;
来源：http://ltj.hysaishi.cn

[Q73] 查看表状态
来源：http://qjx.yongpay.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dtv.wangdashe.top

[Q74] 强制使用索引
来源：http://jjk.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://afm.shuidangran.top

[Q75] 日期格式化
来源：http://vpd.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ntb.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hwb.hnxiangtu.top

[Q76] 按天统计
来源：http://bmd.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gav.dianchejie.cn

[Q77] 时间加减
来源：http://fgs.bbcook.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cdk.0kj1m.cn

[Q78] 当前时间
来源：http://eus.xuanzx.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yjt.cashguo.top

[Q79] 字符串拼接
来源：http://ewm.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gdq.jyoumei.cn

[Q80] 字符串截取
来源：http://lkm.aizwys.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aqp.yangfankeji.com

[Q81] 字符串替换
来源：http://owo.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zrk.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://jqq.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://win.hfpthk.cn

[Q83] 大小写转换
来源：http://axe.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ccu.havefunace.top

[Q84] 去除首尾空格
来源：http://udw.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://ytm.sysykeji.top

[Q85] 数值取整
来源：http://kkk.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jaw.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://yqf.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://klh.ydzc1.top

[Q87] JSON 字段做条件
来源：http://bkw.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eqq.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://feg.svipenyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cjt.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tss.zhoulong.xyz

[Q89] 判断表是否存在
来源：http://pgm.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://shw.cashguo.top

[Q90] 生成序号列
来源：http://rpi.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vgw.svipenyu.cn

================================================================================
来源：http://zxk.sufxvd.cn

R. Bash 专题
来源：http://wuw.pycfn.com

================================================================================
来源：http://zyr.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://aos.sweek.top

#!/usr/bin/env bash
来源：http://xrv.yj20258888.top

set -euo pipefail
来源：http://wri.hesvh.cn

[R02] 变量赋值与使用
来源：http://eue.yj20258.top

name="Tom"; echo "$name"
来源：http://mqw.jqgfzy.top

[R03] 只读变量
来源：http://cjm.sjlbkw.cn

readonly PI=3.14
来源：http://aod.zhongyouzk.top

[R04] 位置参数
来源：http://zyk.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oko.ctjpmb.com

[R05] 参数默认值
来源：http://oiv.zdqjudy.top

name="${1:-default}"
来源：http://ytn.yj202588.top

[R06] 判断命令是否存在
来源：http://oha.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mrt.cucudq.cn

[R07] if 判断文件
来源：http://lxv.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xcs.redwolf501.top

[R08] 数值比较
来源：http://jrw.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://nif.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://wby.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vxq.chenjidiqi.icu

[R10] 正则匹配
来源：http://zrk.vehdjk.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://myr.ctjpmb.com

[R11] case 多分支
来源：http://xhu.havefunace.top

case "$1" in
来源：http://tux.zhengqikj.top

start) echo "启动" ;;
来源：http://vzm.yuanzhike.top

stop)  echo "停止" ;;
来源：http://bez.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://sxe.ctjpmb.com

esac
来源：http://wmc.sufxvd.cn

[R12] for 遍历文件
来源：http://jhr.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://gfh.cqqwz.cn

[R13] for 计数循环
来源：http://wcs.iojbl.cn

for i in {1..10}; do echo "$i"; done
来源：http://qyb.redwolf501.top

[R14] C 风格 for
来源：http://roi.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mia.sjlbkw.cn

[R15] while 逐行读文件
来源：http://scx.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://djw.yvedp.cn

[R16] until 等待条件
来源：http://erm.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xkp.zhaomingkeji.xyz

[R17] 数组定义与取值
来源：http://rjh.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ubm.yuxming.cn

[R18] 遍历数组
来源：http://swk.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ykg.hnqzz.top

[R19] 数组长度
来源：http://rhy.ppjwa.cn

echo "${#arr[@]}"
来源：http://dra.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://cgi.dianchejie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qff.zhengqikj.top

[R21] 字符串长度
来源：http://wso.meibo888.top

echo "${#s}"
来源：http://rdv.yuanzhike.top

[R22] 截取子串
来源：http://man.yangfankeji.com

echo "${s:0:5}"
来源：http://ucd.bbcook.cn

[R23] 字符串替换
来源：http://ltf.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iyk.aibaodan.cn

[R24] 大小写转换
来源：http://waa.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://uhx.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://slt.uphjek.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://gbt.daxiang520.top

[R26] 命令替换
来源：http://kqc.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://kkl.uphjek.com

[R27] 算术展开
来源：http://iwm.316326.xyz

echo $((1 + 2 * 3))
来源：http://bzn.jiagoushi.top

[R28] 浮点运算
来源：http://gzy.chenlongwang.top

echo "scale=2; 10/3" | bc
来源：http://xmu.yueranfly.top

[R29] 定义函数
来源：http://scd.jlsjyb.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tyr.zhongyouzk.top

[R30] 函数返回状态码
来源：http://aio.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://nmc.hongshengwenyu.top

[R31] 局部变量
来源：http://plt.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://ajd.chenlongwang.top

[R32] 参数个数校验
来源：http://wge.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fvk.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://isr.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hsx.xziqi.cn

[R34] 退出时清理
来源：http://ifc.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://snv.dianchejie.cn

[R35] 后台执行并等待
来源：http://ibw.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://hay.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://vpx.smart0.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tzj.ybcxt.top

[R37] 把输出赋给变量
来源：http://lzn.tanke756.top

files=$(ls -1)
来源：http://dgd.meibo888.top

[R38] 管道串联
来源：http://cva.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://nev.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://jbs.havefunace.top

cmd > out.log 2>&1
来源：http://iia.xuanzx.com

[R40] 追加写日志
来源：http://cre.fzhhl.top

echo "log" >> out.log
来源：http://eku.fzhhl.top

[R41] 丢弃输出
来源：http://fpw.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://hhc.hywenlv.cn

[R42] 输入重定向
来源：http://toe.bjfxy.top

wc -l < a.txt
来源：http://mme.xziqi.cn

[R43] 按名字查找文件
来源：http://iik.tarul.cn

find . -name "*.log" -type f
来源：http://eay.dashuyun.cn

[R44] 按修改时间查找
来源：http://aex.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://zrl.bbcook.cn

[R45] 批量删除
来源：http://vcl.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://rpg.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://klb.shzxlz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tzc.snrcjt.cn

[R47] sed 单行替换
来源：http://lzq.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://slt.ivvv.top

[R48] awk 取指定列
来源：http://zlv.ydjk.org.cn

awk '{print $1, $3}' a.txt
来源：http://iul.aizwys.cn

[R49] awk 带条件
来源：http://dvf.yonumen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jtr.zhoulong.xyz

[R50] awk 求和
来源：http://pks.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://ybp.zhijiandao.cn

[R51] 排序去重取前几
来源：http://rhq.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rkh.nanxinkj.top

[R52] 统计行数
来源：http://ajs.xuetiantiany.cn

wc -l a.txt
来源：http://wsl.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://oqj.hcnkem.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zvd.jinqigufen.top

[R54] 比较两个文件
来源：http://lre.pycfn.com

diff a.txt b.txt
来源：http://fuz.hongshengwenyu.top

[R55] 压缩与解压
来源：http://wex.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yrn.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://eha.316326.xyz

scp file user@host:/path/
来源：http://ioe.xziqi.cn

[R57] 远程执行命令
来源：http://mry.zhengqikj.top

ssh user@host 'uptime'
来源：http://hsp.jinqigufen.top

[R58] 下载文件
来源：http://nnv.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qsb.hammf.cn

[R59] 发 POST JSON
来源：http://qju.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://plb.zhiwuduotai.top

[R60] 只看 HTTP 状态码
来源：http://huj.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qke.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://qqe.c1oappe.top

df -h;  du -sh *
来源：http://tcz.yongpay.top

[R62] 找最占空间的文件
来源：http://gqt.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://gbn.hnqzz.top

[R63] 内存与进程
来源：http://ekp.pycfn.com

free -h;  ps aux | grep nginx
来源：http://jxz.0kj1m.cn

[R64] 结束进程
来源：http://sfc.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://mra.yangfankeji.com

[R65] 查看端口占用
来源：http://hse.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hey.fktsv.cn

[R66] 定时任务
来源：http://dyw.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://jzz.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://hgl.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://ujh.ivvv.top

[R68] 计算文件校验值
来源：http://akq.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://qnj.sxryk.cn

[R69] 生成随机密码
来源：http://yeo.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://pqm.aizwys.cn

[R70] 时间戳与互转
来源：http://goi.bbcook.cn

date +%s;  date -d @1700000000
来源：http://beg.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://jvb.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://glf.jqgufenzy.top

[R72] 等待端口就绪
来源：http://dcd.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nrt.sxryk.cn

[R73] 分割大日志
来源：http://pqb.dashuyun.cn

split -l 1000 big.log part_
来源：http://hep.hnxiangtu.top

[R74] 批量重命名
来源：http://fro.c1oappe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yvv.shzxlz.cn

[R75] 导出环境变量
来源：http://cyn.yvedp.cn

export PATH="$HOME/bin:$PATH"
来源：http://goy.9152youxi.cn

[R76] 使用临时文件
来源：http://ugx.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lpy.feifeiyinyue.top

[R77] 读取用户输入
来源：http://ocr.daxiang520.top

read -rp "请输入: " ans
来源：http://snc.yfazqb.com

[R78] 交互式菜单
来源：http://nrb.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://yah.hnqzz.top

[R79] 解析命令行选项
来源：http://qwy.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zyz.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://jxc.tanke756.top

time ./run.sh
来源：http://swm.jiagoushi.top

================================================================================
来源：http://pgi.gzhubu.top

S. C / C++ 专题
来源：http://kjp.chenlongwang.top

================================================================================
来源：http://rlc.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://sfx.vehdjk.com

#include <stdio.h>
来源：http://kgp.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://edy.hnxiangtu.top

[S02] C：变量与格式化输出
来源：http://zpd.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://yjx.fzhhl.top

[S03] C：读入整数
来源：http://oly.zhengqikj.top

int x; scanf("%d", &x);
来源：http://xul.gogol.net.cn

[S04] C：字符串复制
来源：http://cfq.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zqx.c1oappe.top

[S05] C：字符串长度
来源：http://vih.yj202588.top

strlen(s)
来源：http://llh.chenjidiqi.icu

[S06] C：字符串比较
来源：http://hvc.hammf.cn

strcmp(a, b) == 0
来源：http://gpe.ivvv.top

[S07] C：数组遍历求和
来源：http://itw.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wys.jiagoushi.top

[S08] C：动态内存分配与释放
来源：http://wot.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://plb.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://zfr.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vqq.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://jvj.havefunace.top

int *p = &a;  *p = 5;
来源：http://nuq.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://gzg.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://prk.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nqi.jinqigufen.top

fclose(f);
来源：http://cen.pycfn.com

[S12] C：写文件
来源：http://zpa.kuanghao11.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fcp.aibaodan.cn

[S13] C：宏定义
来源：http://lvz.jianghu66.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bzo.birdmap.top

[S14] C：枚举
来源：http://vvl.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://qmj.kuanghao11.cn

[S15] C：类型转换
来源：http://qie.cheryme.top

(double) a / b
来源：http://lbk.gaohongyu789.top

[S16] C：位操作置位
来源：http://qqk.ydzc1.top

x |= (1 << 3);
来源：http://dzm.ybcxt.top

[S17] C：安全拼接字符串
来源：http://dxg.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lcq.iojbl.cn

[S18] C：命令行参数
来源：http://tfw.c1oappe.top


<!-- 参考信息 -->