代发 wailian999

[Q63] 开启事务
来源：http://rpm.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rdi.tian-w.cn

[Q64] 提交事务
来源：http://cum.daria6918.cn

COMMIT;
来源：http://ziv.ppjwa.cn

[Q65] 回滚事务
来源：http://odf.svipenyu.cn

ROLLBACK;
来源：http://kxz.gaohongyu789.top

[Q66] 行锁查询
来源：http://vhj.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jpt.yangfankeji.com

[Q67] 设置隔离级别
来源：http://vjg.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rzo.fehbvm.com

[Q68] 保存点
来源：http://bcq.sysykeji.top

SAVEPOINT sp1;
来源：http://wnd.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://wti.yonumen.top

[Q69] 查看执行计划
来源：http://fib.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lmv.dashuyun.cn

[Q70] 更新统计信息
来源：http://xsr.chenjidiqi.icu

ANALYZE TABLE users;
来源：http://jfs.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://esh.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xqt.ivvv.top

[Q72] 查看索引
来源：http://quw.jinqigufen.top

SHOW INDEX FROM users;
来源：http://ykl.hcnkem.com

[Q73] 查看表状态
来源：http://cpe.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://frt.dashuyun.cn

[Q74] 强制使用索引
来源：http://abz.tian-w.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pzw.sxryk.cn

[Q75] 日期格式化
来源：http://lwi.jianghu66.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://obe.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mse.jinqigufen.top

[Q76] 按天统计
来源：http://jmo.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bch.sufxvd.cn

[Q77] 时间加减
来源：http://rjr.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jfr.hywenlv.cn

[Q78] 当前时间
来源：http://yid.hfpthk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wpu.zhiwuduotai.top

[Q79] 字符串拼接
来源：http://jnv.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aiu.zhiwuduotai.top

[Q80] 字符串截取
来源：http://xcp.vqdsnc.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xvq.nwbrower.top

[Q81] 字符串替换
来源：http://nve.gaohongyu789.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rve.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://fsa.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mqz.ivvv.top

[Q83] 大小写转换
来源：http://kns.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mjw.fzhhl.top

[Q84] 去除首尾空格
来源：http://pqr.yanxiufei.cn

SELECT TRIM(name) FROM users;
来源：http://pqq.zhijiandao.cn

[Q85] 数值取整
来源：http://zng.jiagoushi.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aey.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://yfc.redwolf501.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wjx.nwbrower.top

[Q87] JSON 字段做条件
来源：http://kpg.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wot.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://bod.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hal.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aiz.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://ofc.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ytr.hnxiangtu.top

[Q90] 生成序号列
来源：http://qku.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vos.cashguo.top

================================================================================
来源：http://tmw.andypj.xyz

R. Bash 专题
来源：http://eor.haohaochexian.top

================================================================================
来源：http://vrt.shangyingyoupin.top

[R01] shebang 与严格模式
来源：http://nit.haohaochexian.top

#!/usr/bin/env bash
来源：http://hue.cqqwz.cn

set -euo pipefail
来源：http://pfd.52xcode.cn

[R02] 变量赋值与使用
来源：http://squ.xuetiantiany.cn

name="Tom"; echo "$name"
来源：http://zcm.jinghuilouyu.cn

[R03] 只读变量
来源：http://bos.yvedp.cn

readonly PI=3.14
来源：http://yno.mhx1999.top

[R04] 位置参数
来源：http://rci.aizwys.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kxg.zdqjudy.top

[R05] 参数默认值
来源：http://fjp.wangshuangyany.cn

name="${1:-default}"
来源：http://zgs.9152youxi.cn

[R06] 判断命令是否存在
来源：http://hfg.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ugp.xinyue.icu

[R07] if 判断文件
来源：http://hpr.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gzq.fzhhl.top

[R08] 数值比较
来源：http://wty.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://djg.9152youxi.cn

[R09] 字符串比较
来源：http://qbo.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qwj.yueranfly.top

[R10] 正则匹配
来源：http://exd.yueranfly.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mnr.cdnleiting.top

[R11] case 多分支
来源：http://iou.pycfn.com

case "$1" in
来源：http://ksl.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://uau.chenzaomai.com

stop)  echo "停止" ;;
来源：http://auf.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://fsa.yuanzhike.top

esac
来源：http://agq.sysykeji.top

[R12] for 遍历文件
来源：http://igb.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://dfn.smart0.xyz

[R13] for 计数循环
来源：http://lnh.iojbl.cn

for i in {1..10}; do echo "$i"; done
来源：http://gma.yanxiufei.cn

[R14] C 风格 for
来源：http://ecq.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nwe.yuxming.cn

[R15] while 逐行读文件
来源：http://ygg.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eic.zhoulong.xyz

[R16] until 等待条件
来源：http://plr.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qxp.haohaochexian.top

[R17] 数组定义与取值
来源：http://fpx.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://hox.yfazqb.com

[R18] 遍历数组
来源：http://bqt.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dgm.jinghuilouyu.cn

[R19] 数组长度
来源：http://qfq.dianchejie.cn

echo "${#arr[@]}"
来源：http://zom.wangdashe.top

[R20] 关联数组（字典）
来源：http://pqc.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ihw.zhijiandao.cn

[R21] 字符串长度
来源：http://dmd.hfpthk.cn

echo "${#s}"
来源：http://wcs.zdqjudy.top

[R22] 截取子串
来源：http://zqu.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://gwo.tianlin.xyz

[R23] 字符串替换
来源：http://kam.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zfr.hysaishi.cn

[R24] 大小写转换
来源：http://kal.yj202588.top

echo "${s^^}"; echo "${s,,}"
来源：http://wry.hongshengwenyu.top

[R25] 去后缀 / 去前缀
来源：http://dnf.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://axw.wangshuangyany.cn

[R26] 命令替换
来源：http://orz.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://fpk.hammf.cn

[R27] 算术展开
来源：http://fhw.jianghu66.top

echo $((1 + 2 * 3))
来源：http://qow.jinqigfzy.top

[R28] 浮点运算
来源：http://ogj.yj20258888.top

echo "scale=2; 10/3" | bc
来源：http://jdp.uphjek.com

[R29] 定义函数
来源：http://rua.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vpy.zhijiandao.cn

[R30] 函数返回状态码
来源：http://pls.gaohongyu789.top

f() { return 0; }; f || echo "失败了"
来源：http://iqg.9152youxi.cn

[R31] 局部变量
来源：http://eyv.0kj1m.cn

f() { local x=1; echo "$x"; }
来源：http://hla.mhx1999.top

[R32] 参数个数校验
来源：http://moi.sweek.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ait.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://kqi.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eoh.daria6918.cn

[R34] 退出时清理
来源：http://hyh.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://nuu.tianlin.xyz

[R35] 后台执行并等待
来源：http://qdg.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jcc.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://mry.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qlc.bjfxy.top

[R37] 把输出赋给变量
来源：http://nll.sysykeji.top

files=$(ls -1)
来源：http://doj.guowangkeji.top

[R38] 管道串联
来源：http://rbu.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://bkg.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://uht.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://ryr.vehdjk.com

[R40] 追加写日志
来源：http://rzr.daria6918.cn

echo "log" >> out.log
来源：http://heh.hysaishi.cn

[R41] 丢弃输出
来源：http://orn.pycfn.com

cmd >/dev/null 2>&1
来源：http://ylu.dianchejie.cn

[R42] 输入重定向
来源：http://ecn.dianchejie.cn

wc -l < a.txt
来源：http://aeo.fengsongda.top

[R43] 按名字查找文件
来源：http://rzq.yfazqb.com

find . -name "*.log" -type f
来源：http://ksa.zhongyouzk.top

[R44] 按修改时间查找
来源：http://mad.chenlongwang.top

find . -mtime -7 -type f
来源：http://mjj.nanxinkj.top

[R45] 批量删除
来源：http://kif.uphjek.com

find . -name "*.tmp" -delete
来源：http://psj.guannengcc.top

[R46] 递归替换文件内容
来源：http://oyw.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jpt.svipenyu.cn

[R47] sed 单行替换
来源：http://lhz.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://miu.xuanzx.com

[R48] awk 取指定列
来源：http://fxz.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://zsg.yj20258888.top

[R49] awk 带条件
来源：http://mdw.fanxiaobao.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wha.chenjidiqi.icu

[R50] awk 求和
来源：http://ous.zdqjudy.top

awk '{s += $2} END {print s}' a.txt
来源：http://moi.vehdjk.com

[R51] 排序去重取前几
来源：http://rdz.ehwqpu.com

sort a.txt | uniq -c | sort -rn | head
来源：http://rxg.gotoacloud.top

[R52] 统计行数
来源：http://ngn.gaohongyu789.top

wc -l a.txt
来源：http://ixz.meibo888.top

[R53] 查看文件头与实时尾
来源：http://tbp.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ajh.tarul.cn

[R54] 比较两个文件
来源：http://qvs.jlsjyb.cn

diff a.txt b.txt
来源：http://qda.hfpthk.cn

[R55] 压缩与解压
来源：http://gtr.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yph.wangdashe.top

[R56] 远程拷贝
来源：http://qnl.iojbl.cn

scp file user@host:/path/
来源：http://udw.zhongyouzk.top

[R57] 远程执行命令
来源：http://set.ivvv.top

ssh user@host 'uptime'
来源：http://ohp.jinyuanbaomall.cn

[R58] 下载文件
来源：http://ato.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rrk.c1oappe.top

[R59] 发 POST JSON
来源：http://qzf.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://agv.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://hpt.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cfq.sxryk.cn

[R61] 磁盘占用
来源：http://odg.chenlongwang.top

df -h;  du -sh *
来源：http://zak.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://fcv.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://atd.tianlin.xyz

[R63] 内存与进程
来源：http://fdm.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://bht.hongshengwenyu.top

[R64] 结束进程
来源：http://jxz.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://ceo.quarkkingdee.top

[R65] 查看端口占用
来源：http://tnq.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nai.tianlin.xyz

[R66] 定时任务
来源：http://qaq.52xcode.cn

crontab -e;  crontab -l
来源：http://lpt.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://pax.sjlbkw.cn

openssl rand -hex 16
来源：http://mjn.shzxlz.cn

[R68] 计算文件校验值
来源：http://ufy.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://eug.yj202588.top

[R69] 生成随机密码
来源：http://iyg.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://ors.uphjek.com

[R70] 时间戳与互转
来源：http://iyy.xuetiantiany.cn

date +%s;  date -d @1700000000
来源：http://jkm.cdnleiting.top

[R71] 日期格式化
来源：http://zqk.cqqwz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://urx.zdqjudy.top

[R72] 等待端口就绪
来源：http://wpw.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uyd.yanxiufei.cn

[R73] 分割大日志
来源：http://zkw.yfazqb.com

split -l 1000 big.log part_
来源：http://ncb.xuanzx.com

[R74] 批量重命名
来源：http://wtz.haohaochexian.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fmx.yj20258.top

[R75] 导出环境变量
来源：http://evv.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://vmp.sufxvd.cn

[R76] 使用临时文件
来源：http://vza.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://epp.9152youxi.cn

[R77] 读取用户输入
来源：http://bmm.tarul.cn

read -rp "请输入: " ans
来源：http://ind.zhixingplan.top

[R78] 交互式菜单
来源：http://dkb.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jjw.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://gks.yuxming.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lfo.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://zpk.zhaomingkeji.xyz

time ./run.sh
来源：http://xsm.zhijiandao.cn

================================================================================
来源：http://ptv.0kj1m.cn

S. C / C++ 专题
来源：http://iqe.havefunace.top

================================================================================
来源：http://mnh.hnxiangtu.top

[S01] C：Hello World
来源：http://slc.haohaochexian.top

#include <stdio.h>
来源：http://ptd.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ymm.yonumen.top

[S02] C：变量与格式化输出
来源：http://rzg.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://okk.pengpengdd.cyou

[S03] C：读入整数
来源：http://fap.yuanzhike.top

int x; scanf("%d", &x);
来源：http://pdz.yj202588.top

[S04] C：字符串复制
来源：http://arh.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://aal.quarkkingdee.top

[S05] C：字符串长度
来源：http://abd.shanyushiyangkeji.top

strlen(s)
来源：http://oax.zhengqikj.top

[S06] C：字符串比较
来源：http://ewx.wangdashe.top

strcmp(a, b) == 0
来源：http://svb.yuxming.cn

[S07] C：数组遍历求和
来源：http://jqq.zhaomingkeji.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gzn.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://cbd.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jag.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://zbl.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xzq.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://ttn.sxryk.cn

int *p = &a;  *p = 5;
来源：http://vou.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://fmb.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://hht.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bal.tianlin.xyz

fclose(f);
来源：http://jur.shuidangran.top

[S12] C：写文件
来源：http://exw.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://put.jqgfzy.top

[S13] C：宏定义
来源：http://dic.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ucg.316326.xyz

[S14] C：枚举
来源：http://zph.ehwqpu.com

enum Color { RED, GREEN, BLUE };
来源：http://hgx.ybcxt.top

[S15] C：类型转换
来源：http://niw.sweek.top

(double) a / b
来源：http://msn.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://apl.birdmap.top

x |= (1 << 3);
来源：http://llh.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://tle.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://awe.cucudq.cn

[S18] C：命令行参数
来源：http://jmx.hongshengwenyu.top

int main(int argc, char **argv)
来源：http://lcy.ydzc1.top

[S19] C：快速排序
来源：http://kgd.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://jfi.dianchejie.cn

[S20] C：二分查找
来源：http://brf.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ajo.ehwqpu.com

[S21] C：字符类别判断
来源：http://weu.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yqe.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://vbo.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wne.cqqwz.cn

[S23] C：随机数
来源：http://ncb.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://btf.sysykeji.top

[S24] C：获取本地时间
来源：http://gcg.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iyq.0kj1m.cn

[S25] C：内存拷贝
来源：http://dfs.sufxvd.cn

memcpy(dst, src, n);
来源：http://szk.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://lvf.pycfn.com

memset(a, 0, sizeof a);
来源：http://kwl.bjfxy.top

[S27] C：定义常量
来源：http://bwn.zhaomingkeji.xyz

const double PI = 3.14159;
来源：http://kkz.iojbl.cn

[S28] C：静态变量
来源：http://trr.zhongyouzk.top

static int counter = 0;
来源：http://iig.bbcook.cn

[S29] C：变参函数
来源：http://kut.yangfankeji.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mhd.cdnleiting.top

[S30] C：头文件保护
来源：http://sda.dianchejie.cn

#ifndef X_H
来源：http://xdg.nanxuanxn.top

#define X_H
来源：http://jwj.chenlongwang.top

#endif
来源：http://zhc.tianlin.xyz

[S31] C++：Hello World
来源：http://uoi.aibaodan.cn

#include <iostream>
来源：http://dkl.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://ego.xylfe.cn

[S32] C++：字符串
来源：http://sjs.xylfe.cn

std::string s = "hi";  s += "!";
来源：http://rqb.gotoacloud.top


<!-- 参考信息 -->