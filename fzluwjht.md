代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ucr.daria6918.cn

[Q58] 累计求和
来源：http://utc.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nzs.aizwys.cn

[Q59] 分组内累计
来源：http://csx.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://huc.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://hcc.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zrl.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qop.cucudq.cn

[Q61] 移动平均
来源：http://czg.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://awn.nanxinkj.top

[Q62] 分组占比
来源：http://tym.iojbl.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qyy.epnwcf.com

[Q63] 开启事务
来源：http://kcs.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://vmg.zhiwuduotai.top

[Q64] 提交事务
来源：http://eed.haohaochexian.top

COMMIT;
来源：http://hcc.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://zsg.cashguo.top

ROLLBACK;
来源：http://kur.yuanzhike.top

[Q66] 行锁查询
来源：http://udq.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jrf.aibaodan.cn

[Q67] 设置隔离级别
来源：http://sdm.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hxh.shuidangran.top

[Q68] 保存点
来源：http://swd.smart0.xyz

SAVEPOINT sp1;
来源：http://ybk.aibaodan.cn

ROLLBACK TO sp1;
来源：http://ctz.52xcode.cn

[Q69] 查看执行计划
来源：http://oyg.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uaz.tian-w.cn

[Q70] 更新统计信息
来源：http://isz.yanxiufei.cn

ANALYZE TABLE users;
来源：http://clf.gotoacloud.top

[Q71] 查看建表语句
来源：http://xwm.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lcd.cucudq.cn

[Q72] 查看索引
来源：http://gzt.zdqjudy.top

SHOW INDEX FROM users;
来源：http://afg.xziqi.cn

[Q73] 查看表状态
来源：http://kiz.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nmn.sysykeji.top

[Q74] 强制使用索引
来源：http://uoa.yj20258.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fqp.jlsjyb.cn

[Q75] 日期格式化
来源：http://ntj.mhx1999.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cux.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sai.kuanghao11.cn

[Q76] 按天统计
来源：http://hbn.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://svk.chenjidiqi.icu

[Q77] 时间加减
来源：http://zwv.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vcq.gotoacloud.top

[Q78] 当前时间
来源：http://rdy.jinqigfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bwx.yongpay.top

[Q79] 字符串拼接
来源：http://hjm.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dre.daria6918.cn

[Q80] 字符串截取
来源：http://fjh.zdbjq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lya.sjlbkw.cn

[Q81] 字符串替换
来源：http://nmd.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://caz.redwolf501.top

[Q82] 字符长度与字节长度
来源：http://xmz.guowangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zol.zhixingplan.top

[Q83] 大小写转换
来源：http://uwg.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wkn.mhx1999.top

[Q84] 去除首尾空格
来源：http://bdj.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://qiv.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://qfs.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gtj.nwbrower.top

[Q86] 读取 JSON 字段
来源：http://mza.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://awd.meibo888.top

[Q87] JSON 字段做条件
来源：http://oce.yj202588.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://egr.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://qyp.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tlj.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dwy.pengpengdd.cyou

[Q89] 判断表是否存在
来源：http://kik.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uct.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://tet.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rnh.fzhhl.top

================================================================================
来源：http://ogm.zdqjudy.top

R. Bash 专题
来源：http://usm.zdbjq.cn

================================================================================
来源：http://zcp.snrcjt.cn

[R01] shebang 与严格模式
来源：http://plx.aizwys.cn

#!/usr/bin/env bash
来源：http://lwr.svipenyu.cn

set -euo pipefail
来源：http://jbs.xziqi.cn

[R02] 变量赋值与使用
来源：http://bai.yangfankeji.com

name="Tom"; echo "$name"
来源：http://orp.meibo888.top

[R03] 只读变量
来源：http://bnl.sjlbkw.cn

readonly PI=3.14
来源：http://knv.9152youxi.cn

[R04] 位置参数
来源：http://jjv.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xfm.zdqjudy.top

[R05] 参数默认值
来源：http://vsy.tianlin.xyz

name="${1:-default}"
来源：http://wzy.hywenlv.cn

[R06] 判断命令是否存在
来源：http://nmg.wangshuangyany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zcp.havefunace.top

[R07] if 判断文件
来源：http://qas.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://npd.chenzaomai.com

[R08] 数值比较
来源：http://ogm.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://edb.ppjwa.cn

[R09] 字符串比较
来源：http://eml.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rai.nanxuanxn.top

[R10] 正则匹配
来源：http://cuw.jqgfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kmb.yangfankeji.com

[R11] case 多分支
来源：http://fxk.jianghu66.top

case "$1" in
来源：http://zmg.cdnleiting.top

start) echo "启动" ;;
来源：http://xfs.uphjek.com

stop)  echo "停止" ;;
来源：http://dsm.aizwys.cn

*)     echo "未知命令" ;;
来源：http://tmq.yfazqb.com

esac
来源：http://bwk.zhengqikj.top

[R12] for 遍历文件
来源：http://nfy.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://sbb.redwolf501.top

[R13] for 计数循环
来源：http://nof.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://frs.shzxlz.cn

[R14] C 风格 for
来源：http://pac.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://voq.zhaomingkeji.xyz

[R15] while 逐行读文件
来源：http://zen.hnxiangtu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nho.sxryk.cn

[R16] until 等待条件
来源：http://srw.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fiv.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://mvf.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://fxp.jinqigufen.top

[R18] 遍历数组
来源：http://xws.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vdx.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://syu.cashguo.top

echo "${#arr[@]}"
来源：http://moy.9152youxi.cn

[R20] 关联数组（字典）
来源：http://dui.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dwr.tanke756.top

[R21] 字符串长度
来源：http://isv.ppjwa.cn

echo "${#s}"
来源：http://dax.meibo888.top

[R22] 截取子串
来源：http://owu.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://rsb.hywenlv.cn

[R23] 字符串替换
来源：http://vpl.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fdm.yj20258.top

[R24] 大小写转换
来源：http://fzg.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://vxo.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://dkm.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://ihr.yangfankeji.com

[R26] 命令替换
来源：http://qhc.ydzc1.top

now=$(date +%F); echo "$now"
来源：http://pbc.wangshuangyany.cn

[R27] 算术展开
来源：http://see.ybcxt.top

echo $((1 + 2 * 3))
来源：http://kzk.316326.xyz

[R28] 浮点运算
来源：http://wvi.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://uyz.jyoumei.cn

[R29] 定义函数
来源：http://wqt.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gyh.yj20258888.top

[R30] 函数返回状态码
来源：http://wcj.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://hil.sufxvd.cn

[R31] 局部变量
来源：http://irv.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://pwb.yfazqb.com

[R32] 参数个数校验
来源：http://lrd.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iui.sweek.top

[R33] 捕获错误并提示行号
来源：http://car.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bkr.nwbrower.top

[R34] 退出时清理
来源：http://bpi.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://hlh.haohaochexian.top

[R35] 后台执行并等待
来源：http://ksl.birdmap.top

sleep 5 & pid=$!; wait "$pid"
来源：http://aly.aizwys.cn

[R36] 并发执行多个任务
来源：http://fbl.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eld.chenzaomai.com

[R37] 把输出赋给变量
来源：http://nqb.xingfuxueyuan.xyz

files=$(ls -1)
来源：http://ygj.cheryme.top

[R38] 管道串联
来源：http://sox.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://cuy.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://nba.shuidangran.top

cmd > out.log 2>&1
来源：http://gwo.ctjpmb.com

[R40] 追加写日志
来源：http://qic.sysykeji.top

echo "log" >> out.log
来源：http://ggv.yangfankeji.com

[R41] 丢弃输出
来源：http://mky.ybcxt.top

cmd >/dev/null 2>&1
来源：http://ydz.yangfankeji.com

[R42] 输入重定向
来源：http://wyr.andypj.xyz

wc -l < a.txt
来源：http://xwg.pycfn.com

[R43] 按名字查找文件
来源：http://fkm.c1oappe.top

find . -name "*.log" -type f
来源：http://gsn.iojbl.cn

[R44] 按修改时间查找
来源：http://vln.9152youxi.cn

find . -mtime -7 -type f
来源：http://vnu.quarkkingdee.top

[R45] 批量删除
来源：http://zkq.hcnkem.com

find . -name "*.tmp" -delete
来源：http://vaz.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://vqg.jinqigufen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://acm.birdmap.top

[R47] sed 单行替换
来源：http://hta.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rez.xuanzx.com

[R48] awk 取指定列
来源：http://bqe.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://sql.quarkkingdee.top

[R49] awk 带条件
来源：http://pxy.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nzk.yuxming.cn

[R50] awk 求和
来源：http://jrz.yongpay.top

awk '{s += $2} END {print s}' a.txt
来源：http://sbu.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://mip.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://sac.52xcode.cn

[R52] 统计行数
来源：http://gbm.guannengcc.top

wc -l a.txt
来源：http://qpy.gzhubu.top

[R53] 查看文件头与实时尾
来源：http://bji.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ujv.tianlin.xyz

[R54] 比较两个文件
来源：http://smf.haohaochexian.top

diff a.txt b.txt
来源：http://nhm.hywenlv.cn

[R55] 压缩与解压
来源：http://yyf.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ybp.svipenyu.cn

[R56] 远程拷贝
来源：http://kih.pengpengdd.cyou

scp file user@host:/path/
来源：http://ytd.pengpengdd.cyou

[R57] 远程执行命令
来源：http://gji.zhengqikj.top

ssh user@host 'uptime'
来源：http://kep.316326.xyz

[R58] 下载文件
来源：http://kqr.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ovl.zhongyouzk.top

[R59] 发 POST JSON
来源：http://ozi.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://byk.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://qlq.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hra.sysykeji.top

[R61] 磁盘占用
来源：http://iju.xziqi.cn

df -h;  du -sh *
来源：http://gxh.guowangkeji.top

[R62] 找最占空间的文件
来源：http://kuy.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://dal.tanke756.top

[R63] 内存与进程
来源：http://sod.fengsongda.top

free -h;  ps aux | grep nginx
来源：http://nwb.yonumen.top

[R64] 结束进程
来源：http://ody.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://vcu.smart0.xyz

[R65] 查看端口占用
来源：http://yng.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oba.feifeiyinyue.top

[R66] 定时任务
来源：http://pjt.smart0.xyz

crontab -e;  crontab -l
来源：http://rds.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://ykt.yj20258888.top

openssl rand -hex 16
来源：http://nav.cqqwz.cn

[R68] 计算文件校验值
来源：http://msc.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://yoo.yvedp.cn

[R69] 生成随机密码
来源：http://yhm.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://tzz.0kj1m.cn

[R70] 时间戳与互转
来源：http://qfu.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://mtm.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://cya.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lyz.316326.xyz

[R72] 等待端口就绪
来源：http://dah.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fvi.yuanzhike.top

[R73] 分割大日志
来源：http://cpo.xylfe.cn

split -l 1000 big.log part_
来源：http://ndb.birdmap.top

[R74] 批量重命名
来源：http://cjx.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wsv.zhoulong.xyz

[R75] 导出环境变量
来源：http://jdv.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://tyn.yvedp.cn

[R76] 使用临时文件
来源：http://jzk.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dvh.shangyingyoupin.top

[R77] 读取用户输入
来源：http://inu.chenzaomai.com

read -rp "请输入: " ans
来源：http://nrb.ivvv.top

[R78] 交互式菜单
来源：http://hum.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nhp.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://jcx.sysykeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rhe.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://jwm.cashguo.top

time ./run.sh
来源：http://wmf.bbcook.cn

================================================================================
来源：http://oim.daxiang520.top

S. C / C++ 专题
来源：http://vnv.ctjpmb.com

================================================================================
来源：http://zdy.yvedp.cn

[S01] C：Hello World
来源：http://uvc.snrcjt.cn

#include <stdio.h>
来源：http://jff.kuanghao11.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wjs.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://jnz.fengsongda.top

int a = 10; printf("%d\n", a);
来源：http://wbk.nanxuanxn.top

[S03] C：读入整数
来源：http://utr.sufxvd.cn

int x; scanf("%d", &x);
来源：http://xnh.havefunace.top

[S04] C：字符串复制
来源：http://szj.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://pkt.bjfxy.top

[S05] C：字符串长度
来源：http://ftq.fengsongda.top

strlen(s)
来源：http://dqu.zdbjq.cn

[S06] C：字符串比较
来源：http://elm.jyoumei.cn

strcmp(a, b) == 0
来源：http://xzl.316326.xyz

[S07] C：数组遍历求和
来源：http://bcz.fanxiaobao.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tow.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://nep.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hyf.hongshengwenyu.top

[S09] C：结构体定义与初始化
来源：http://kzb.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iyd.ctjpmb.com

[S10] C：指针与解引用
来源：http://gfi.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://zwe.andypj.xyz

[S11] C：逐行读文件
来源：http://fai.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://mwk.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://cgz.52xcode.cn

fclose(f);
来源：http://hmb.c1oappe.top

[S12] C：写文件
来源：http://rev.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fqx.tian-w.cn

[S13] C：宏定义
来源：http://eau.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ltb.yj20258888.top

[S14] C：枚举
来源：http://mqf.epnwcf.com

enum Color { RED, GREEN, BLUE };
来源：http://klr.cdnleiting.top

[S15] C：类型转换
来源：http://olk.zhixingplan.top

(double) a / b
来源：http://gci.jqgfzy.top

[S16] C：位操作置位
来源：http://fyg.guannengcc.top

x |= (1 << 3);
来源：http://udc.aibaodan.cn

[S17] C：安全拼接字符串
来源：http://vop.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://czm.birdmap.top

[S18] C：命令行参数
来源：http://fax.hysaishi.cn

int main(int argc, char **argv)
来源：http://kbc.zhixingplan.top

[S19] C：快速排序
来源：http://xsn.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://nje.tarul.cn

[S20] C：二分查找
来源：http://uvb.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ibv.kuanghao11.cn

[S21] C：字符类别判断
来源：http://utp.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tnt.chenzaomai.com

[S22] C：字符串转数字
来源：http://aak.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cow.redwolf501.top

[S23] C：随机数
来源：http://tmu.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jxo.gzhubu.top

[S24] C：获取本地时间
来源：http://ypy.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rno.ppjwa.cn

[S25] C：内存拷贝
来源：http://gpq.zhiwuduotai.top

memcpy(dst, src, n);
来源：http://tsb.yvedp.cn

[S26] C：内存清零
来源：http://xql.vehdjk.com

memset(a, 0, sizeof a);
来源：http://zhv.andypj.xyz

[S27] C：定义常量
来源：http://wpg.daxiang520.top

const double PI = 3.14159;
来源：http://ren.bbcook.cn

[S28] C：静态变量
来源：http://kgo.gzhubu.top


<!-- 参考信息 -->