代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zct.jinqigfzy.top

[Q54] 清空表
来源：http://ipa.yueranfly.top

TRUNCATE TABLE logs;
来源：http://csl.sufxvd.cn

[Q55] 排名（并列占位）
来源：http://cye.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gtd.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://ixz.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tih.havefunace.top

[Q57] 行号
来源：http://kfq.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xqp.chenlongwang.top

[Q58] 累计求和
来源：http://cqi.chenjidiqi.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gbu.fanxiaobao.xyz

[Q59] 分组内累计
来源：http://bqb.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zlo.ydjk.org.cn

[Q60] 取上一行 / 下一行
来源：http://eto.nwbrower.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dnb.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yzr.tianlin.xyz

[Q61] 移动平均
来源：http://gyw.shanyushiyangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yqj.vqdsnc.cn

[Q62] 分组占比
来源：http://iag.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qte.quarkkingdee.top

[Q63] 开启事务
来源：http://vrm.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ttq.quarkkingdee.top

[Q64] 提交事务
来源：http://eac.yanxiufei.cn

COMMIT;
来源：http://ure.bjfxy.top

[Q65] 回滚事务
来源：http://pup.smart0.xyz

ROLLBACK;
来源：http://ojr.xinyue.icu

[Q66] 行锁查询
来源：http://eua.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vwz.fehbvm.com

[Q67] 设置隔离级别
来源：http://wlg.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xie.c1oappe.top

[Q68] 保存点
来源：http://aqw.fehbvm.com

SAVEPOINT sp1;
来源：http://ylv.tianlin.xyz

ROLLBACK TO sp1;
来源：http://xqg.bbcook.cn

[Q69] 查看执行计划
来源：http://cth.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://knm.iojbl.cn

[Q70] 更新统计信息
来源：http://ozr.ydzc1.top

ANALYZE TABLE users;
来源：http://via.yangfankeji.com

[Q71] 查看建表语句
来源：http://frw.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fve.guannengcc.top

[Q72] 查看索引
来源：http://tsu.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://ijo.0kj1m.cn

[Q73] 查看表状态
来源：http://uvh.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tle.shzxlz.cn

[Q74] 强制使用索引
来源：http://wvm.ivvv.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://igu.snrcjt.cn

[Q75] 日期格式化
来源：http://xma.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rlw.aizwys.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rmo.zhongyouzk.top

[Q76] 按天统计
来源：http://ecg.hysaishi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ayx.shuidangran.top

[Q77] 时间加减
来源：http://gua.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yqz.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://cch.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ods.jianghu66.top

[Q79] 字符串拼接
来源：http://uat.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iig.ppjwa.cn

[Q80] 字符串截取
来源：http://qhf.tian-w.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://utp.fengsongda.top

[Q81] 字符串替换
来源：http://wvw.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nns.yj20258.top

[Q82] 字符长度与字节长度
来源：http://dqt.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xoi.snrcjt.cn

[Q83] 大小写转换
来源：http://gjp.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tvc.tian-w.cn

[Q84] 去除首尾空格
来源：http://cbh.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://sdq.zhixingplan.top

[Q85] 数值取整
来源：http://bfz.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jlr.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://xic.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hlh.fanxiaobao.xyz

[Q87] JSON 字段做条件
来源：http://gzd.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://twd.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://yhr.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xoq.zdbjq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tud.fktsv.cn

[Q89] 判断表是否存在
来源：http://cql.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ivv.nanxinkj.top

[Q90] 生成序号列
来源：http://ysi.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://krk.jinqigfzy.top

================================================================================
来源：http://kkf.jqgfzy.top

R. Bash 专题
来源：http://gzj.ybcxt.top

================================================================================
来源：http://fgl.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://ltj.sysykeji.top

#!/usr/bin/env bash
来源：http://inh.52xcode.cn

set -euo pipefail
来源：http://fuv.snrcjt.cn

[R02] 变量赋值与使用
来源：http://ahc.xylfe.cn

name="Tom"; echo "$name"
来源：http://hfk.yj20258888.top

[R03] 只读变量
来源：http://tbj.aibaodan.cn

readonly PI=3.14
来源：http://bic.tanke756.top

[R04] 位置参数
来源：http://mdk.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fxz.pengpengdd.cyou

[R05] 参数默认值
来源：http://bnc.xuetiantiany.cn

name="${1:-default}"
来源：http://cns.shanyushiyangtech.top

[R06] 判断命令是否存在
来源：http://umz.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vla.guannengcc.top

[R07] if 判断文件
来源：http://odr.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lvv.snrcjt.cn

[R08] 数值比较
来源：http://ycu.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ujn.gotoacloud.top

[R09] 字符串比较
来源：http://loh.jianghu66.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gdm.jiagoushi.top

[R10] 正则匹配
来源：http://kco.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iao.uphjek.com

[R11] case 多分支
来源：http://fyg.jinqigfzy.top

case "$1" in
来源：http://mhs.pengpengdd.cyou

start) echo "启动" ;;
来源：http://awj.ehwqpu.com

stop)  echo "停止" ;;
来源：http://afq.pycfn.com

*)     echo "未知命令" ;;
来源：http://wir.ehwqpu.com

esac
来源：http://dwy.dianchejie.cn

[R12] for 遍历文件
来源：http://gnv.ydzc1.top

for f in *.txt; do echo "$f"; done
来源：http://gwa.meibo888.top

[R13] for 计数循环
来源：http://ydf.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://iim.shzxlz.cn

[R14] C 风格 for
来源：http://kiu.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://heq.gotoacloud.top

[R15] while 逐行读文件
来源：http://emr.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://csb.tanke756.top

[R16] until 等待条件
来源：http://bkk.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ewy.ivvv.top

[R17] 数组定义与取值
来源：http://goj.yonumen.top

arr=(a b c); echo "${arr[0]}"
来源：http://mrp.zdqjudy.top

[R18] 遍历数组
来源：http://kir.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hie.52xcode.cn

[R19] 数组长度
来源：http://eku.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://klj.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://anf.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uww.daria6918.cn

[R21] 字符串长度
来源：http://uvp.yangfankeji.com

echo "${#s}"
来源：http://ztr.andypj.xyz

[R22] 截取子串
来源：http://oer.zhengqikj.top

echo "${s:0:5}"
来源：http://wdi.hcnkem.com

[R23] 字符串替换
来源：http://qus.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ifk.ivvv.top

[R24] 大小写转换
来源：http://iwy.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://sye.zhoulong.xyz

[R25] 去后缀 / 去前缀
来源：http://igl.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dur.ehwqpu.com

[R26] 命令替换
来源：http://adr.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://hjd.yj202588.top

[R27] 算术展开
来源：http://tnb.xuanzx.com

echo $((1 + 2 * 3))
来源：http://zzf.jlsjyb.cn

[R28] 浮点运算
来源：http://pfd.gaohongyu789.top

echo "scale=2; 10/3" | bc
来源：http://ymv.wangshuangyany.cn

[R29] 定义函数
来源：http://vsz.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cml.gaohongyu789.top

[R30] 函数返回状态码
来源：http://oub.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://nco.sweek.top

[R31] 局部变量
来源：http://jnb.zhijiandao.cn

f() { local x=1; echo "$x"; }
来源：http://mwn.ctjpmb.com

[R32] 参数个数校验
来源：http://yng.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ypf.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://ocb.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ysg.feifeiyinyue.top

[R34] 退出时清理
来源：http://xip.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://tpk.andypj.xyz

[R35] 后台执行并等待
来源：http://hng.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rrh.52xcode.cn

[R36] 并发执行多个任务
来源：http://xhv.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fbi.0kj1m.cn

[R37] 把输出赋给变量
来源：http://lhi.0kj1m.cn

files=$(ls -1)
来源：http://seh.jlsjyb.cn

[R38] 管道串联
来源：http://cbp.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://waz.hammf.cn

[R39] 重定向标准输出与错误
来源：http://vvz.gogol.net.cn

cmd > out.log 2>&1
来源：http://dqo.cqqwz.cn

[R40] 追加写日志
来源：http://mqq.ybcxt.top

echo "log" >> out.log
来源：http://zvo.fengsongda.top

[R41] 丢弃输出
来源：http://jke.fehbvm.com

cmd >/dev/null 2>&1
来源：http://auu.fehbvm.com

[R42] 输入重定向
来源：http://fhz.jianghu66.top

wc -l < a.txt
来源：http://qrn.tianlin.xyz

[R43] 按名字查找文件
来源：http://dyn.mhx1999.top

find . -name "*.log" -type f
来源：http://dae.meibo888.top

[R44] 按修改时间查找
来源：http://osy.cqqwz.cn

find . -mtime -7 -type f
来源：http://uom.havefunace.top

[R45] 批量删除
来源：http://bmw.xinyue.icu

find . -name "*.tmp" -delete
来源：http://lym.cqqwz.cn

[R46] 递归替换文件内容
来源：http://mzg.hcnkem.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://byc.zdqjudy.top

[R47] sed 单行替换
来源：http://kuq.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://wcv.epnwcf.com

[R48] awk 取指定列
来源：http://xhk.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://kxt.sufxvd.cn

[R49] awk 带条件
来源：http://pak.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kpf.guannengcc.top

[R50] awk 求和
来源：http://wkk.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://igq.xziqi.cn

[R51] 排序去重取前几
来源：http://hdv.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rtf.andypj.xyz

[R52] 统计行数
来源：http://tdd.xinyue.icu

wc -l a.txt
来源：http://ghv.gzhubu.top

[R53] 查看文件头与实时尾
来源：http://njh.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wna.yonumen.top

[R54] 比较两个文件
来源：http://rmp.xuetiantiany.cn

diff a.txt b.txt
来源：http://jtz.redwolf501.top

[R55] 压缩与解压
来源：http://isn.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ymk.tian-w.cn

[R56] 远程拷贝
来源：http://rrk.nanxuanxn.top

scp file user@host:/path/
来源：http://kpp.chenlongwang.top

[R57] 远程执行命令
来源：http://kel.chenlongwang.top

ssh user@host 'uptime'
来源：http://tfe.yangfankeji.com

[R58] 下载文件
来源：http://flo.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mpd.gzhubu.top

[R59] 发 POST JSON
来源：http://yns.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yin.sweek.top

[R60] 只看 HTTP 状态码
来源：http://dgk.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://klt.daria6918.cn

[R61] 磁盘占用
来源：http://cpd.jiagoushi.top

df -h;  du -sh *
来源：http://lxk.ctjpmb.com

[R62] 找最占空间的文件
来源：http://wnn.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://tty.hysaishi.cn

[R63] 内存与进程
来源：http://bsj.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://jmd.tanke756.top

[R64] 结束进程
来源：http://yeq.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://ips.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://wqv.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rmd.wangdashe.top

[R66] 定时任务
来源：http://lbv.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://zlh.smart0.xyz

[R67] 生成随机十六进制串
来源：http://sgb.mhx1999.top

openssl rand -hex 16
来源：http://kca.wangdashe.top

[R68] 计算文件校验值
来源：http://mkf.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://zzt.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://afr.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://zan.epnwcf.com

[R70] 时间戳与互转
来源：http://ojk.fzhhl.top

date +%s;  date -d @1700000000
来源：http://nzg.fehbvm.com

[R71] 日期格式化
来源：http://wmx.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://cak.hfpthk.cn

[R72] 等待端口就绪
来源：http://wlm.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://kmk.sysykeji.top

[R73] 分割大日志
来源：http://cpb.yj20258.top

split -l 1000 big.log part_
来源：http://pfu.meibo888.top

[R74] 批量重命名
来源：http://vvv.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wni.kuanghao11.cn

[R75] 导出环境变量
来源：http://vpu.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://ynm.vqdsnc.cn

[R76] 使用临时文件
来源：http://oya.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://czn.yongpay.top

[R77] 读取用户输入
来源：http://gmi.svipenyu.cn

read -rp "请输入: " ans
来源：http://ssm.xuetiantiany.cn

[R78] 交互式菜单
来源：http://jom.quarkkingdee.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oap.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://rxi.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kcf.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://bau.iojbl.cn

time ./run.sh
来源：http://edc.daria6918.cn

================================================================================
来源：http://ore.yuanzhike.top

S. C / C++ 专题
来源：http://ubu.daria6918.cn

================================================================================
来源：http://tbb.snrcjt.cn

[S01] C：Hello World
来源：http://jar.guannengcc.top

#include <stdio.h>
来源：http://xbb.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ymb.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://oau.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://mjz.cashguo.top

[S03] C：读入整数
来源：http://sex.sweek.top

int x; scanf("%d", &x);
来源：http://chx.nanxinkj.top

[S04] C：字符串复制
来源：http://cgj.xziqi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mgn.jqgfzy.top

[S05] C：字符串长度
来源：http://toc.jinqigufen.top

strlen(s)
来源：http://bhb.hfpthk.cn

[S06] C：字符串比较
来源：http://lnm.havefunace.top

strcmp(a, b) == 0
来源：http://uet.zhixingplan.top

[S07] C：数组遍历求和
来源：http://bud.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cfg.aibaodan.cn

[S08] C：动态内存分配与释放
来源：http://nyz.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cwi.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://gtf.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xph.ehwqpu.com

[S10] C：指针与解引用
来源：http://pgu.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://uqu.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://qlv.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://rar.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://aoj.tanke756.top

fclose(f);
来源：http://wir.yanxiufei.cn

[S12] C：写文件
来源：http://vei.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pvy.hywenlv.cn

[S13] C：宏定义
来源：http://mlw.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eoc.vqdsnc.cn

[S14] C：枚举
来源：http://scv.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://pvy.xziqi.cn

[S15] C：类型转换
来源：http://ofd.sweek.top

(double) a / b
来源：http://wmc.aibaodan.cn

[S16] C：位操作置位
来源：http://url.redwolf501.top

x |= (1 << 3);
来源：http://ilp.gzhubu.top

[S17] C：安全拼接字符串
来源：http://gqy.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rbw.kuanghao11.cn

[S18] C：命令行参数
来源：http://jnl.fengsongda.top

int main(int argc, char **argv)
来源：http://jzt.zhoulong.xyz

[S19] C：快速排序
来源：http://wwf.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://qjc.jqgufenzy.top

[S20] C：二分查找
来源：http://xyh.gaohongyu789.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tll.jiagoushi.top

[S21] C：字符类别判断
来源：http://wsq.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cbt.nanxuanxn.top

[S22] C：字符串转数字
来源：http://ukw.pycfn.com

atoi("42");  strtod("3.14", NULL);
来源：http://qsx.hnqzz.top

[S23] C：随机数
来源：http://uum.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cug.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://kap.tianlin.xyz


<!-- 参考信息 -->