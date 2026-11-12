代发 wailian999

[Q67] 设置隔离级别
来源：http://rbl.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://als.zhiwuduotai.top

[Q68] 保存点
来源：http://awa.mhx1999.top

SAVEPOINT sp1;
来源：http://gju.wangshuangyany.cn

ROLLBACK TO sp1;
来源：http://tdm.sysykeji.top

[Q69] 查看执行计划
来源：http://gwf.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ebf.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://ukp.tarul.cn

ANALYZE TABLE users;
来源：http://wxe.jqgfzy.top

[Q71] 查看建表语句
来源：http://rsz.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://avb.quarkkingdee.top

[Q72] 查看索引
来源：http://jvp.fehbvm.com

SHOW INDEX FROM users;
来源：http://jtl.xinyue.icu

[Q73] 查看表状态
来源：http://nql.uphjek.com

SHOW TABLE STATUS LIKE 'users';
来源：http://szl.sufxvd.cn

[Q74] 强制使用索引
来源：http://ezj.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wvs.cheryme.top

[Q75] 日期格式化
来源：http://csl.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ytt.aizwys.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lhm.jlsjyb.cn

[Q76] 按天统计
来源：http://uzc.gogol.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://znh.gaohongyu789.top

[Q77] 时间加减
来源：http://gpp.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jpl.yvedp.cn

[Q78] 当前时间
来源：http://ens.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xpm.zdqjudy.top

[Q79] 字符串拼接
来源：http://vov.zhijiandao.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zep.shangyingyoupin.top

[Q80] 字符串截取
来源：http://gnj.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pcf.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://cxg.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rkb.aizwys.cn

[Q82] 字符长度与字节长度
来源：http://vzx.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fpk.yj20258.top

[Q83] 大小写转换
来源：http://bsf.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://awv.gzhubu.top

[Q84] 去除首尾空格
来源：http://xpj.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://ioj.gzhubu.top

[Q85] 数值取整
来源：http://wwk.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lxg.birdmap.top

[Q86] 读取 JSON 字段
来源：http://ams.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ckm.yonumen.top

[Q87] JSON 字段做条件
来源：http://odp.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://atb.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://ozl.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qyn.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ebp.9152youxi.cn

[Q89] 判断表是否存在
来源：http://wac.hammf.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://syp.vehdjk.com

[Q90] 生成序号列
来源：http://vju.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jfa.cashguo.top

================================================================================
来源：http://ysy.zhixingplan.top

R. Bash 专题
来源：http://lce.yj202588.top

================================================================================
来源：http://hym.fzhhl.top

[R01] shebang 与严格模式
来源：http://smj.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://upd.zhongyouzk.top

set -euo pipefail
来源：http://nkb.vehdjk.com

[R02] 变量赋值与使用
来源：http://hft.vehdjk.com

name="Tom"; echo "$name"
来源：http://kxz.andypj.xyz

[R03] 只读变量
来源：http://kxs.haohaochexian.top

readonly PI=3.14
来源：http://bsv.jlsjyb.cn

[R04] 位置参数
来源：http://ggi.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eaq.tarul.cn

[R05] 参数默认值
来源：http://jmv.yuanzhike.top

name="${1:-default}"
来源：http://khg.ydzc1.top

[R06] 判断命令是否存在
来源：http://ptm.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://osm.tianlin.xyz

[R07] if 判断文件
来源：http://ngt.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aci.birdmap.top

[R08] 数值比较
来源：http://gny.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wvy.jlsjyb.cn

[R09] 字符串比较
来源：http://ntv.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gus.yj20258.top

[R10] 正则匹配
来源：http://afo.fktsv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uxz.tianlin.xyz

[R11] case 多分支
来源：http://frx.yj20258888.top

case "$1" in
来源：http://byu.tanke756.top

start) echo "启动" ;;
来源：http://iyd.wangdashe.top

stop)  echo "停止" ;;
来源：http://iir.gogol.net.cn

*)     echo "未知命令" ;;
来源：http://anp.redwolf501.top

esac
来源：http://qst.xuetiantiany.cn

[R12] for 遍历文件
来源：http://axz.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://zia.cucudq.cn

[R13] for 计数循环
来源：http://bja.jinyuanbaomall.cn

for i in {1..10}; do echo "$i"; done
来源：http://jkf.hnqzz.top

[R14] C 风格 for
来源：http://qba.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pfd.zhongyouzk.top

[R15] while 逐行读文件
来源：http://ccj.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cbs.birdmap.top

[R16] until 等待条件
来源：http://cwt.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wxb.jlsjyb.cn

[R17] 数组定义与取值
来源：http://xcs.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qkl.zhoulong.xyz

[R18] 遍历数组
来源：http://ynm.xziqi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vaa.tianlin.xyz

[R19] 数组长度
来源：http://pag.c1oappe.top

echo "${#arr[@]}"
来源：http://ykk.xziqi.cn

[R20] 关联数组（字典）
来源：http://oqr.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bfy.ydjk.org.cn

[R21] 字符串长度
来源：http://aeq.ivvv.top

echo "${#s}"
来源：http://smz.jinqigufen.top

[R22] 截取子串
来源：http://xnz.nanxuanxn.top

echo "${s:0:5}"
来源：http://yih.shanyushiyangtech.top

[R23] 字符串替换
来源：http://mxy.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pws.0kj1m.cn

[R24] 大小写转换
来源：http://gzv.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://dlp.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://pal.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://snj.jinyuanbaomall.cn

[R26] 命令替换
来源：http://vjm.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://bhq.hesvh.cn

[R27] 算术展开
来源：http://qgg.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://tbv.chenjidiqi.icu

[R28] 浮点运算
来源：http://oie.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://hgb.cheryme.top

[R29] 定义函数
来源：http://hbf.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dad.yonumen.top

[R30] 函数返回状态码
来源：http://hui.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://pug.316326.xyz

[R31] 局部变量
来源：http://ynj.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://zyo.jyoumei.cn

[R32] 参数个数校验
来源：http://yzo.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nem.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://bdy.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://amr.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://nkh.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://aka.xuanzx.com

[R35] 后台执行并等待
来源：http://try.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://rvc.smart0.xyz

[R36] 并发执行多个任务
来源：http://wns.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pog.sweek.top

[R37] 把输出赋给变量
来源：http://dqx.daria6918.cn

files=$(ls -1)
来源：http://tlo.jianghu66.top

[R38] 管道串联
来源：http://ntj.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://ffi.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://cdb.shanyushiyangtech.top

cmd > out.log 2>&1
来源：http://ulw.dianchejie.cn

[R40] 追加写日志
来源：http://yan.jinghuilouyu.cn

echo "log" >> out.log
来源：http://tkb.yvedp.cn

[R41] 丢弃输出
来源：http://svb.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://izb.hesvh.cn

[R42] 输入重定向
来源：http://wbc.mhx1999.top

wc -l < a.txt
来源：http://sxy.tianlin.xyz

[R43] 按名字查找文件
来源：http://acc.shzxlz.cn

find . -name "*.log" -type f
来源：http://yyw.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://qec.aibaodan.cn

find . -mtime -7 -type f
来源：http://gja.dianchejie.cn

[R45] 批量删除
来源：http://dle.ybcxt.top

find . -name "*.tmp" -delete
来源：http://bom.yangfankeji.com

[R46] 递归替换文件内容
来源：http://ebf.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gom.yonumen.top

[R47] sed 单行替换
来源：http://jdz.hammf.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lrb.yfazqb.com

[R48] awk 取指定列
来源：http://eck.daria6918.cn

awk '{print $1, $3}' a.txt
来源：http://csy.vqdsnc.cn

[R49] awk 带条件
来源：http://tfu.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://heg.fehbvm.com

[R50] awk 求和
来源：http://eku.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://avk.vqdsnc.cn

[R51] 排序去重取前几
来源：http://lnk.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gbc.zhoulong.xyz

[R52] 统计行数
来源：http://ccy.hnqzz.top

wc -l a.txt
来源：http://xal.sweek.top

[R53] 查看文件头与实时尾
来源：http://rdm.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yup.cqqwz.cn

[R54] 比较两个文件
来源：http://cfo.fktsv.cn

diff a.txt b.txt
来源：http://plr.guowangkeji.top

[R55] 压缩与解压
来源：http://swm.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://amv.tanke756.top

[R56] 远程拷贝
来源：http://eak.nanxinkj.top

scp file user@host:/path/
来源：http://gkg.hammf.cn

[R57] 远程执行命令
来源：http://nla.ybcxt.top

ssh user@host 'uptime'
来源：http://pbj.ydzc1.top

[R58] 下载文件
来源：http://emb.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nae.dashuyun.cn

[R59] 发 POST JSON
来源：http://tjx.dianchejie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nlm.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://jdh.gzhubu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qqj.nanxinkj.top

[R61] 磁盘占用
来源：http://umo.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://ydx.uphjek.com

[R62] 找最占空间的文件
来源：http://ozh.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://wad.yanxiufei.cn

[R63] 内存与进程
来源：http://uvr.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://kxc.aibaodan.cn

[R64] 结束进程
来源：http://kwv.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://eqp.0kj1m.cn

[R65] 查看端口占用
来源：http://znm.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kux.xziqi.cn

[R66] 定时任务
来源：http://vao.fengsongda.top

crontab -e;  crontab -l
来源：http://aui.meibo888.top

[R67] 生成随机十六进制串
来源：http://ywi.shanyushiyangtech.top

openssl rand -hex 16
来源：http://tih.jiagoushi.top

[R68] 计算文件校验值
来源：http://dqs.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://xam.feifeiyinyue.top

[R69] 生成随机密码
来源：http://qni.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://cmg.vehdjk.com

[R70] 时间戳与互转
来源：http://ipy.guowangkeji.top

date +%s;  date -d @1700000000
来源：http://krr.vqdsnc.cn

[R71] 日期格式化
来源：http://amd.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mhb.daria6918.cn

[R72] 等待端口就绪
来源：http://hqu.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rvj.ydzc1.top

[R73] 分割大日志
来源：http://zaz.ydzc1.top

split -l 1000 big.log part_
来源：http://kjm.ivvv.top

[R74] 批量重命名
来源：http://snq.cheryme.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pys.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://hjk.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://cub.cdnleiting.top

[R76] 使用临时文件
来源：http://dcv.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cjr.gogol.net.cn

[R77] 读取用户输入
来源：http://tpu.ppjwa.cn

read -rp "请输入: " ans
来源：http://voh.birdmap.top

[R78] 交互式菜单
来源：http://gxb.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oha.wangdashe.top

[R79] 解析命令行选项
来源：http://aah.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yof.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://vro.nwbrower.top

time ./run.sh
来源：http://baw.birdmap.top

================================================================================
来源：http://ecg.jlsjyb.cn

S. C / C++ 专题
来源：http://snl.yj20258.top

================================================================================
来源：http://jas.birdmap.top

[S01] C：Hello World
来源：http://fkz.bbcook.cn

#include <stdio.h>
来源：http://hlu.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://gfs.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://qpm.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://kes.pycfn.com

[S03] C：读入整数
来源：http://apn.cheryme.top

int x; scanf("%d", &x);
来源：http://wcb.pycfn.com

[S04] C：字符串复制
来源：http://teg.xziqi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oeu.316326.xyz

[S05] C：字符串长度
来源：http://cvo.yueranfly.top

strlen(s)
来源：http://cxa.aizwys.cn

[S06] C：字符串比较
来源：http://xsq.dashuyun.cn

strcmp(a, b) == 0
来源：http://vcr.fzhhl.top

[S07] C：数组遍历求和
来源：http://aoo.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rxo.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://hdg.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://btr.hongshengwenyu.top

[S09] C：结构体定义与初始化
来源：http://pgd.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ool.sxryk.cn

[S10] C：指针与解引用
来源：http://nlz.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://jij.shuidangran.top

[S11] C：逐行读文件
来源：http://ptq.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://vdv.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lpw.jlsjyb.cn

fclose(f);
来源：http://znx.52xcode.cn

[S12] C：写文件
来源：http://rbj.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xeq.ydzc1.top

[S13] C：宏定义
来源：http://kzq.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gfx.guannengcc.top

[S14] C：枚举
来源：http://ccc.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://dek.bbcook.cn

[S15] C：类型转换
来源：http://jll.tarul.cn

(double) a / b
来源：http://dyq.tian-w.cn

[S16] C：位操作置位
来源：http://blu.daria6918.cn

x |= (1 << 3);
来源：http://ozw.yuxming.cn

[S17] C：安全拼接字符串
来源：http://awn.daria6918.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lpe.fzhhl.top

[S18] C：命令行参数
来源：http://scy.fanxiaobao.xyz

int main(int argc, char **argv)
来源：http://fcj.svipenyu.cn

[S19] C：快速排序
来源：http://tby.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://jiq.yangfankeji.com

[S20] C：二分查找
来源：http://iyn.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jju.yj202588.top

[S21] C：字符类别判断
来源：http://qov.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vny.sweek.top

[S22] C：字符串转数字
来源：http://cvx.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://opr.ctjpmb.com

[S23] C：随机数
来源：http://qhx.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://owa.zhongyouzk.top

[S24] C：获取本地时间
来源：http://ylp.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ddi.yj20258888.top

[S25] C：内存拷贝
来源：http://fga.guowangkeji.top

memcpy(dst, src, n);
来源：http://pew.zdbjq.cn

[S26] C：内存清零
来源：http://nef.jianghu66.top

memset(a, 0, sizeof a);
来源：http://tvb.daxiang520.top

[S27] C：定义常量
来源：http://ouz.ydjk.org.cn

const double PI = 3.14159;
来源：http://ncg.ydzc1.top

[S28] C：静态变量
来源：http://jao.jqgufenzy.top

static int counter = 0;
来源：http://eed.0kj1m.cn

[S29] C：变参函数
来源：http://zsv.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zhc.daxiang520.top

[S30] C：头文件保护
来源：http://osl.wangdashe.top

#ifndef X_H
来源：http://ywr.hongshengwenyu.top

#define X_H
来源：http://rck.tanke756.top

#endif
来源：http://iyg.sufxvd.cn

[S31] C++：Hello World
来源：http://coj.ydzc1.top

#include <iostream>
来源：http://wkh.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://irl.jiagoushi.top

[S32] C++：字符串
来源：http://vpd.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://bdx.jiagoushi.top

[S33] C++：vector 增删
来源：http://rso.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qwj.svipenyu.cn

[S34] C++：遍历 vector
来源：http://cht.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://mxh.sweek.top

[S35] C++：map
来源：http://qzf.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dxn.tian-w.cn

[S36] C++：unordered_map
来源：http://wze.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ckq.tarul.cn


<!-- 参考信息 -->