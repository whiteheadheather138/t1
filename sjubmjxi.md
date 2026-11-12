代发 wailian999

ANALYZE TABLE users;
来源：http://udc.bbcook.cn

[Q71] 查看建表语句
来源：http://beg.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://elj.chenjidiqi.icu

[Q72] 查看索引
来源：http://jes.zhixingplan.top

SHOW INDEX FROM users;
来源：http://ssd.sysykeji.top

[Q73] 查看表状态
来源：http://krk.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nlc.cucudq.cn

[Q74] 强制使用索引
来源：http://han.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dvv.fehbvm.com

[Q75] 日期格式化
来源：http://oow.redwolf501.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://egs.epnwcf.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dld.yueranfly.top

[Q76] 按天统计
来源：http://sgy.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qju.jinghuilouyu.cn

[Q77] 时间加减
来源：http://ngz.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ovl.feifeiyinyue.top

[Q78] 当前时间
来源：http://syu.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hwv.sxryk.cn

[Q79] 字符串拼接
来源：http://tmd.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://shk.iojbl.cn

[Q80] 字符串截取
来源：http://oxr.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lsu.ivvv.top

[Q81] 字符串替换
来源：http://kzm.jlsjyb.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rxq.cdnleiting.top

[Q82] 字符长度与字节长度
来源：http://zxn.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yox.cheryme.top

[Q83] 大小写转换
来源：http://ftq.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jai.xuanzx.com

[Q84] 去除首尾空格
来源：http://gow.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://igc.shzxlz.cn

[Q85] 数值取整
来源：http://opc.sxryk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ejh.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://vgu.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dxq.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://pxz.ywan-chungtsiang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xcd.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://ndf.zhongyouzk.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lke.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zdd.yuanzhike.top

[Q89] 判断表是否存在
来源：http://yoq.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ppy.yueranfly.top

[Q90] 生成序号列
来源：http://yen.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://trn.daria6918.cn

================================================================================
来源：http://ozp.cheryme.top

R. Bash 专题
来源：http://ite.meibo888.top

================================================================================
来源：http://evz.zhaomingkeji.xyz

[R01] shebang 与严格模式
来源：http://krr.bbcook.cn

#!/usr/bin/env bash
来源：http://vpx.daria6918.cn

set -euo pipefail
来源：http://nvt.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://kvs.nanxinkj.top

name="Tom"; echo "$name"
来源：http://hen.smart0.xyz

[R03] 只读变量
来源：http://gcw.ppjwa.cn

readonly PI=3.14
来源：http://vkr.snrcjt.cn

[R04] 位置参数
来源：http://mnx.kuanghao11.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zeb.yj20258888.top

[R05] 参数默认值
来源：http://vyy.zhaomingkeji.xyz

name="${1:-default}"
来源：http://vah.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://hma.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oek.yueranfly.top

[R07] if 判断文件
来源：http://kyo.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rcu.jlsjyb.cn

[R08] 数值比较
来源：http://lhp.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hjq.nanxuanxn.top

[R09] 字符串比较
来源：http://llu.daria6918.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vjb.jqgfzy.top

[R10] 正则匹配
来源：http://zrm.yuanzhike.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uow.jyoumei.cn

[R11] case 多分支
来源：http://tsh.yonumen.top

case "$1" in
来源：http://wrj.hcnkem.com

start) echo "启动" ;;
来源：http://fzf.epnwcf.com

stop)  echo "停止" ;;
来源：http://oyh.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://noo.hesvh.cn

esac
来源：http://jpq.sweek.top

[R12] for 遍历文件
来源：http://xjr.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://vhp.hnqzz.top

[R13] for 计数循环
来源：http://izt.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://twz.yfazqb.com

[R14] C 风格 for
来源：http://swu.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uhn.daxiang520.top

[R15] while 逐行读文件
来源：http://ztg.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tkr.guowangkeji.top

[R16] until 等待条件
来源：http://dts.chenjidiqi.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rxj.nanxuanxn.top

[R17] 数组定义与取值
来源：http://ioz.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://jir.yj20258888.top

[R18] 遍历数组
来源：http://cqk.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eym.kuanghao11.cn

[R19] 数组长度
来源：http://xcn.zhaomingkeji.xyz

echo "${#arr[@]}"
来源：http://pci.xuanzx.com

[R20] 关联数组（字典）
来源：http://mlg.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eki.epnwcf.com

[R21] 字符串长度
来源：http://cpe.zhaomingkeji.xyz

echo "${#s}"
来源：http://dkf.shuidangran.top

[R22] 截取子串
来源：http://tka.xuetiantiany.cn

echo "${s:0:5}"
来源：http://ayx.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://ify.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xwt.gzhubu.top

[R24] 大小写转换
来源：http://igy.zhengqikj.top

echo "${s^^}"; echo "${s,,}"
来源：http://bfe.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://ook.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dyq.bjfxy.top

[R26] 命令替换
来源：http://bwd.shuidangran.top

now=$(date +%F); echo "$now"
来源：http://qrn.havefunace.top

[R27] 算术展开
来源：http://ojj.ybcxt.top

echo $((1 + 2 * 3))
来源：http://zxd.sysykeji.top

[R28] 浮点运算
来源：http://dyi.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://vph.zycfv.cn

[R29] 定义函数
来源：http://eol.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bei.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://soa.ydjk.org.cn

f() { return 0; }; f || echo "失败了"
来源：http://ysq.sxryk.cn

[R31] 局部变量
来源：http://ctf.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://aci.kuanghao11.cn

[R32] 参数个数校验
来源：http://vyx.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uov.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://bps.hammf.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zyn.hfpthk.cn

[R34] 退出时清理
来源：http://qkw.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://zbo.yfazqb.com

[R35] 后台执行并等待
来源：http://efg.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ipv.jyoumei.cn

[R36] 并发执行多个任务
来源：http://gbo.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bxu.chenlongwang.top

[R37] 把输出赋给变量
来源：http://mdp.cucudq.cn

files=$(ls -1)
来源：http://fac.fehbvm.com

[R38] 管道串联
来源：http://btm.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://nbm.yongpay.top

[R39] 重定向标准输出与错误
来源：http://cvd.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://mvr.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://dtq.nwbrower.top

echo "log" >> out.log
来源：http://vsc.xuetiantiany.cn

[R41] 丢弃输出
来源：http://hid.xuanzx.com

cmd >/dev/null 2>&1
来源：http://pvw.nanxinkj.top

[R42] 输入重定向
来源：http://gem.guowangkeji.top

wc -l < a.txt
来源：http://bdb.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://jnm.yj20258.top

find . -name "*.log" -type f
来源：http://kbk.ybcxt.top

[R44] 按修改时间查找
来源：http://tpo.fktsv.cn

find . -mtime -7 -type f
来源：http://ein.jqgfzy.top

[R45] 批量删除
来源：http://lbj.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://ngt.zhaomingkeji.xyz

[R46] 递归替换文件内容
来源：http://evj.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kkl.dianchejie.cn

[R47] sed 单行替换
来源：http://xpm.hnqzz.top

sed -i 's/foo/bar/g' a.txt
来源：http://bih.yvedp.cn

[R48] awk 取指定列
来源：http://xuo.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://luz.sweek.top

[R49] awk 带条件
来源：http://qbg.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ciq.zhixingplan.top

[R50] awk 求和
来源：http://mjt.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://xtn.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://kuv.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://whm.jianghu66.top

[R52] 统计行数
来源：http://wrx.jyoumei.cn

wc -l a.txt
来源：http://inv.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://tfx.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://duh.pycfn.com

[R54] 比较两个文件
来源：http://zzv.dashuyun.cn

diff a.txt b.txt
来源：http://wdn.yuxming.cn

[R55] 压缩与解压
来源：http://mwz.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ltz.hcnkem.com

[R56] 远程拷贝
来源：http://gej.sufxvd.cn

scp file user@host:/path/
来源：http://qps.zhiwuduotai.top

[R57] 远程执行命令
来源：http://ewf.gzhubu.top

ssh user@host 'uptime'
来源：http://gja.redwolf501.top

[R58] 下载文件
来源：http://tfk.haohaochexian.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mtk.uphjek.com

[R59] 发 POST JSON
来源：http://kfg.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zqo.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://uot.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mtv.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://rse.jqgufenzy.top

df -h;  du -sh *
来源：http://jrd.hesvh.cn

[R62] 找最占空间的文件
来源：http://jkn.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://and.ctjpmb.com

[R63] 内存与进程
来源：http://gpe.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://edc.yanxiufei.cn

[R64] 结束进程
来源：http://dsf.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://crl.yfazqb.com

[R65] 查看端口占用
来源：http://jxw.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uqq.jlsjyb.cn

[R66] 定时任务
来源：http://byd.dianchejie.cn

crontab -e;  crontab -l
来源：http://dlb.chenlongwang.top

[R67] 生成随机十六进制串
来源：http://vvp.cashguo.top

openssl rand -hex 16
来源：http://bde.kuanghao11.cn

[R68] 计算文件校验值
来源：http://mhy.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://rdg.xylfe.cn

[R69] 生成随机密码
来源：http://thi.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://xnl.aibaodan.cn

[R70] 时间戳与互转
来源：http://ezc.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://svn.ydjk.org.cn

[R71] 日期格式化
来源：http://cvg.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://faa.jqgfzy.top

[R72] 等待端口就绪
来源：http://rpi.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pvd.52xcode.cn

[R73] 分割大日志
来源：http://zix.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://lkr.jinghuilouyu.cn

[R74] 批量重命名
来源：http://qbl.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gol.pengpengdd.cyou

[R75] 导出环境变量
来源：http://sva.shanyushiyangtech.top

export PATH="$HOME/bin:$PATH"
来源：http://bqp.shuidangran.top

[R76] 使用临时文件
来源：http://rnk.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qmh.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://pwx.gotoacloud.top

read -rp "请输入: " ans
来源：http://xsk.zdqjudy.top

[R78] 交互式菜单
来源：http://tvv.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yir.hnxiangtu.top

[R79] 解析命令行选项
来源：http://qwq.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wur.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://lph.hammf.cn

time ./run.sh
来源：http://goe.gotoacloud.top

================================================================================
来源：http://pfl.zhiwuduotai.top

S. C / C++ 专题
来源：http://xmi.iojbl.cn

================================================================================
来源：http://jhs.guowangkeji.top

[S01] C：Hello World
来源：http://uce.yuanzhike.top

#include <stdio.h>
来源：http://qsi.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xvz.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://zmf.316326.xyz

int a = 10; printf("%d\n", a);
来源：http://vno.jqgfzy.top

[S03] C：读入整数
来源：http://zbd.dashuyun.cn

int x; scanf("%d", &x);
来源：http://mfa.cdnleiting.top

[S04] C：字符串复制
来源：http://yer.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://ewo.cqqwz.cn

[S05] C：字符串长度
来源：http://vqh.zdbjq.cn

strlen(s)
来源：http://wpk.chenjidiqi.icu

[S06] C：字符串比较
来源：http://rdp.sjlbkw.cn

strcmp(a, b) == 0
来源：http://ooy.fehbvm.com

[S07] C：数组遍历求和
来源：http://svl.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kqf.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://qif.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://brr.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://wgg.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dik.cheryme.top

[S10] C：指针与解引用
来源：http://njl.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://dxy.ydjk.org.cn

[S11] C：逐行读文件
来源：http://psz.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://njg.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://cmm.andypj.xyz

fclose(f);
来源：http://wbw.kuanghao11.cn

[S12] C：写文件
来源：http://eoo.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gud.hcnkem.com

[S13] C：宏定义
来源：http://uwg.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hsa.wangdashe.top

[S14] C：枚举
来源：http://neg.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://jog.shanyushiyangtech.top

[S15] C：类型转换
来源：http://tcw.gaohongyu789.top

(double) a / b
来源：http://duh.uphjek.com

[S16] C：位操作置位
来源：http://tlp.tanke756.top

x |= (1 << 3);
来源：http://myp.sxryk.cn

[S17] C：安全拼接字符串
来源：http://zcs.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vez.yuanzhike.top

[S18] C：命令行参数
来源：http://jso.fzhhl.top

int main(int argc, char **argv)
来源：http://wjq.cashguo.top

[S19] C：快速排序
来源：http://nxp.birdmap.top

qsort(a, n, sizeof(int), cmp);
来源：http://gee.gotoacloud.top

[S20] C：二分查找
来源：http://utl.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ris.jinqigufen.top

[S21] C：字符类别判断
来源：http://qhu.jyoumei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oip.ydjk.org.cn

[S22] C：字符串转数字
来源：http://zzg.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://xgn.daria6918.cn

[S23] C：随机数
来源：http://gsa.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://rxe.gaohongyu789.top

[S24] C：获取本地时间
来源：http://sbl.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rrv.cdnleiting.top

[S25] C：内存拷贝
来源：http://aaz.jqgfzy.top

memcpy(dst, src, n);
来源：http://irm.hfpthk.cn

[S26] C：内存清零
来源：http://htx.xinyue.icu

memset(a, 0, sizeof a);
来源：http://byn.jianghu66.top

[S27] C：定义常量
来源：http://kpf.hnqzz.top

const double PI = 3.14159;
来源：http://vxd.kuanghao11.cn

[S28] C：静态变量
来源：http://yct.hongshengwenyu.top

static int counter = 0;
来源：http://yzv.guowangkeji.top

[S29] C：变参函数
来源：http://zxk.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gah.chenjidiqi.icu

[S30] C：头文件保护
来源：http://xsk.redwolf501.top

#ifndef X_H
来源：http://wkl.daxiang520.top

#define X_H
来源：http://bcj.fehbvm.com

#endif
来源：http://cxz.jinqigfzy.top

[S31] C++：Hello World
来源：http://meq.xuanzx.com

#include <iostream>
来源：http://jre.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://fzg.sweek.top

[S32] C++：字符串
来源：http://uau.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://rxl.zycfv.cn

[S33] C++：vector 增删
来源：http://fsu.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nbi.vqdsnc.cn

[S34] C++：遍历 vector
来源：http://ovb.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://uda.jinghuilouyu.cn

[S35] C++：map
来源：http://okg.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uzi.xylfe.cn

[S36] C++：unordered_map
来源：http://sam.yj20258888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gcx.gzhubu.top

[S37] C++：set
来源：http://hej.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zne.guowangkeji.top

[S38] C++：排序
来源：http://ghb.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://aoj.guannengcc.top

[S39] C++：自定义比较器排序
来源：http://kcv.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zkm.sjlbkw.cn

[S40] C++：查找元素
来源：http://lgm.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://msl.jianghu66.top


<!-- 参考信息 -->