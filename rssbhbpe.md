代发 wailian999

ROLLBACK TO sp1;
来源：http://oaq.hesvh.cn

[Q69] 查看执行计划
来源：http://oig.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ctl.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://sue.zycfv.cn

ANALYZE TABLE users;
来源：http://hmx.hysaishi.cn

[Q71] 查看建表语句
来源：http://rud.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ooe.9152youxi.cn

[Q72] 查看索引
来源：http://one.vehdjk.com

SHOW INDEX FROM users;
来源：http://wgj.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://vxe.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fdv.ppjwa.cn

[Q74] 强制使用索引
来源：http://djg.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vte.9152youxi.cn

[Q75] 日期格式化
来源：http://qvx.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vpo.xingfuxueyuan.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wpq.jinghuilouyu.cn

[Q76] 按天统计
来源：http://cju.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cfw.hammf.cn

[Q77] 时间加减
来源：http://ydx.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iln.zhongyouzk.top

[Q78] 当前时间
来源：http://uap.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ffg.c1oappe.top

[Q79] 字符串拼接
来源：http://yvk.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sdr.dianchejie.cn

[Q80] 字符串截取
来源：http://ymr.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eey.sysykeji.top

[Q81] 字符串替换
来源：http://gth.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ysg.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://wzy.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jtt.chenzaomai.com

[Q83] 大小写转换
来源：http://wqe.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sur.svipenyu.cn

[Q84] 去除首尾空格
来源：http://uyg.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://zhx.chenzaomai.com

[Q85] 数值取整
来源：http://hfv.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jcb.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://vad.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mvc.zycfv.cn

[Q87] JSON 字段做条件
来源：http://imb.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xjt.yvedp.cn

[Q88] 行转列（条件聚合）
来源：http://qrt.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sny.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oer.yangfankeji.com

[Q89] 判断表是否存在
来源：http://fdz.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bof.cdnleiting.top

[Q90] 生成序号列
来源：http://nri.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://csd.daria6918.cn

================================================================================
来源：http://aob.jinghuilouyu.cn

R. Bash 专题
来源：http://jdp.pengpengdd.cyou

================================================================================
来源：http://cbw.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://yku.cdnleiting.top

#!/usr/bin/env bash
来源：http://tac.nanxinkj.top

set -euo pipefail
来源：http://hvp.daria6918.cn

[R02] 变量赋值与使用
来源：http://pyc.fktsv.cn

name="Tom"; echo "$name"
来源：http://qdg.zdbjq.cn

[R03] 只读变量
来源：http://tix.ybcxt.top

readonly PI=3.14
来源：http://vwh.gotoacloud.top

[R04] 位置参数
来源：http://ubf.hongshengwenyu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bto.vehdjk.com

[R05] 参数默认值
来源：http://xcr.yonumen.top

name="${1:-default}"
来源：http://hyw.c1oappe.top

[R06] 判断命令是否存在
来源：http://nlp.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rzw.0kj1m.cn

[R07] if 判断文件
来源：http://kgk.havefunace.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://upl.fzhhl.top

[R08] 数值比较
来源：http://eef.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kcv.uphjek.com

[R09] 字符串比较
来源：http://now.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fko.fengsongda.top

[R10] 正则匹配
来源：http://okn.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bqr.gaohongyu789.top

[R11] case 多分支
来源：http://tid.zhaomingkeji.xyz

case "$1" in
来源：http://uuo.yj20258888.top

start) echo "启动" ;;
来源：http://txj.yueranfly.top

stop)  echo "停止" ;;
来源：http://jlf.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://ghy.cqqwz.cn

esac
来源：http://whf.daxiang520.top

[R12] for 遍历文件
来源：http://hob.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://jid.zhixingplan.top

[R13] for 计数循环
来源：http://dom.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://prr.sjlbkw.cn

[R14] C 风格 for
来源：http://fsx.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wal.mhx1999.top

[R15] while 逐行读文件
来源：http://lsr.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oao.jinqigufen.top

[R16] until 等待条件
来源：http://zfg.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bdr.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://bov.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://qnz.ivvv.top

[R18] 遍历数组
来源：http://rmw.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xiu.sufxvd.cn

[R19] 数组长度
来源：http://gil.aibaodan.cn

echo "${#arr[@]}"
来源：http://hra.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://lda.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oly.9152youxi.cn

[R21] 字符串长度
来源：http://hcp.hongshengwenyu.top

echo "${#s}"
来源：http://cla.yangfankeji.com

[R22] 截取子串
来源：http://zpi.ywan-chungtsiang.top

echo "${s:0:5}"
来源：http://lto.sweek.top

[R23] 字符串替换
来源：http://usf.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gyg.nanxinkj.top

[R24] 大小写转换
来源：http://onu.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nnf.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://wgz.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dfw.zhoulong.xyz

[R26] 命令替换
来源：http://dqn.chenzaomai.com

now=$(date +%F); echo "$now"
来源：http://cgr.daria6918.cn

[R27] 算术展开
来源：http://khu.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://eih.aibaodan.cn

[R28] 浮点运算
来源：http://dbc.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://nhp.yonumen.top

[R29] 定义函数
来源：http://pia.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vbs.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://ntp.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://olx.chenzaomai.com

[R31] 局部变量
来源：http://nss.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://gvz.uphjek.com

[R32] 参数个数校验
来源：http://zln.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xpm.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://dip.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oor.zhiwuduotai.top

[R34] 退出时清理
来源：http://wfw.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://jlf.dashuyun.cn

[R35] 后台执行并等待
来源：http://ufl.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://cem.yangfankeji.com

[R36] 并发执行多个任务
来源：http://atq.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://typ.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://bnz.yonumen.top

files=$(ls -1)
来源：http://jgk.yj202588.top

[R38] 管道串联
来源：http://ltq.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://rsv.shangyingyoupin.top

[R39] 重定向标准输出与错误
来源：http://fkc.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://bwf.yangfankeji.com

[R40] 追加写日志
来源：http://ffh.ydjk.org.cn

echo "log" >> out.log
来源：http://amq.nwbrower.top

[R41] 丢弃输出
来源：http://gap.daria6918.cn

cmd >/dev/null 2>&1
来源：http://laa.jqgfzy.top

[R42] 输入重定向
来源：http://plj.gaohongyu789.top

wc -l < a.txt
来源：http://oah.guowangkeji.top

[R43] 按名字查找文件
来源：http://whb.zdbjq.cn

find . -name "*.log" -type f
来源：http://qsa.yangfankeji.com

[R44] 按修改时间查找
来源：http://pbj.daxiang520.top

find . -mtime -7 -type f
来源：http://erm.dianchejie.cn

[R45] 批量删除
来源：http://niq.c1oappe.top

find . -name "*.tmp" -delete
来源：http://trm.fktsv.cn

[R46] 递归替换文件内容
来源：http://pci.fanxiaobao.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://acn.zhongyouzk.top

[R47] sed 单行替换
来源：http://ilz.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://mje.dianchejie.cn

[R48] awk 取指定列
来源：http://wme.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://wnh.feifeiyinyue.top

[R49] awk 带条件
来源：http://dwn.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wzv.yj20258888.top

[R50] awk 求和
来源：http://vip.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rwq.yj20258888.top

[R51] 排序去重取前几
来源：http://oxl.xuetiantiany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fhn.cashguo.top

[R52] 统计行数
来源：http://cuz.zhiwuduotai.top

wc -l a.txt
来源：http://pwz.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://upm.cashguo.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ryc.aibaodan.cn

[R54] 比较两个文件
来源：http://koh.hysaishi.cn

diff a.txt b.txt
来源：http://gzm.xuanzx.com

[R55] 压缩与解压
来源：http://hky.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uur.cqqwz.cn

[R56] 远程拷贝
来源：http://coh.ppjwa.cn

scp file user@host:/path/
来源：http://yao.316326.xyz

[R57] 远程执行命令
来源：http://zkm.hnxiangtu.top

ssh user@host 'uptime'
来源：http://mdx.hammf.cn

[R58] 下载文件
来源：http://ref.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oow.sufxvd.cn

[R59] 发 POST JSON
来源：http://qrt.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ydg.cucudq.cn

[R60] 只看 HTTP 状态码
来源：http://alb.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kwg.vqdsnc.cn

[R61] 磁盘占用
来源：http://ipy.fanxiaobao.xyz

df -h;  du -sh *
来源：http://fun.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://gia.fehbvm.com

du -ah . | sort -rh | head -10
来源：http://zdo.quarkkingdee.top

[R63] 内存与进程
来源：http://zzx.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://mrl.nwbrower.top

[R64] 结束进程
来源：http://bds.xuanzx.com

kill -9 $(pgrep -f app.py)
来源：http://xjk.smart0.xyz

[R65] 查看端口占用
来源：http://ulz.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ras.chenlongwang.top

[R66] 定时任务
来源：http://joo.hnqzz.top

crontab -e;  crontab -l
来源：http://bhn.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://gnd.ybcxt.top

openssl rand -hex 16
来源：http://gix.zhaomingkeji.xyz

[R68] 计算文件校验值
来源：http://khy.gogol.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ipz.yuanzhike.top

[R69] 生成随机密码
来源：http://xld.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://uni.havefunace.top

[R70] 时间戳与互转
来源：http://lyt.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://fms.chenjidiqi.icu

[R71] 日期格式化
来源：http://lba.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qiq.zhiwuduotai.top

[R72] 等待端口就绪
来源：http://jar.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://juk.zhiwuduotai.top

[R73] 分割大日志
来源：http://gyl.yangfankeji.com

split -l 1000 big.log part_
来源：http://hlc.zycfv.cn

[R74] 批量重命名
来源：http://gxc.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vuh.epnwcf.com

[R75] 导出环境变量
来源：http://jdx.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://jem.dianchejie.cn

[R76] 使用临时文件
来源：http://uua.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xvv.hywenlv.cn

[R77] 读取用户输入
来源：http://jjj.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://gjj.uphjek.com

[R78] 交互式菜单
来源：http://sdy.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qci.zhengqikj.top

[R79] 解析命令行选项
来源：http://tmr.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jxn.yj20258.top

[R80] 查看脚本执行耗时
来源：http://wvf.ehwqpu.com

time ./run.sh
来源：http://fog.pengpengdd.cyou

================================================================================
来源：http://owm.shuidangran.top

S. C / C++ 专题
来源：http://cvj.fanxiaobao.xyz

================================================================================
来源：http://dfk.wangdashe.top

[S01] C：Hello World
来源：http://fou.redwolf501.top

#include <stdio.h>
来源：http://dry.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ido.shuidangran.top

[S02] C：变量与格式化输出
来源：http://ehl.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://qca.zhiwuduotai.top

[S03] C：读入整数
来源：http://epe.yj20258.top

int x; scanf("%d", &x);
来源：http://gww.chenlongwang.top

[S04] C：字符串复制
来源：http://ffc.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://ief.xinyue.icu

[S05] C：字符串长度
来源：http://lam.zhixingplan.top

strlen(s)
来源：http://lqo.hfpthk.cn

[S06] C：字符串比较
来源：http://vpf.hnxiangtu.top

strcmp(a, b) == 0
来源：http://lcq.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://gqc.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bdk.316326.xyz

[S08] C：动态内存分配与释放
来源：http://kqw.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vgw.shangyingyoupin.top

[S09] C：结构体定义与初始化
来源：http://iba.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qfx.guowangkeji.top

[S10] C：指针与解引用
来源：http://ypm.aizwys.cn

int *p = &a;  *p = 5;
来源：http://sfl.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://pck.iojbl.cn

FILE *f = fopen("a.txt", "r");
来源：http://ust.yangfankeji.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://khj.hesvh.cn

fclose(f);
来源：http://vch.yongpay.top

[S12] C：写文件
来源：http://amh.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ayb.guowangkeji.top

[S13] C：宏定义
来源：http://ddi.gogol.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pkr.nanxuanxn.top

[S14] C：枚举
来源：http://lmi.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://jnm.epnwcf.com

[S15] C：类型转换
来源：http://mdk.shuidangran.top

(double) a / b
来源：http://hdn.wangshuangyany.cn

[S16] C：位操作置位
来源：http://tuf.ctjpmb.com

x |= (1 << 3);
来源：http://eju.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://xmz.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ixf.jianghu66.top

[S18] C：命令行参数
来源：http://jya.sjlbkw.cn

int main(int argc, char **argv)
来源：http://rjp.ydjk.org.cn

[S19] C：快速排序
来源：http://hqp.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qia.bbcook.cn

[S20] C：二分查找
来源：http://hea.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://poz.nanxinkj.top

[S21] C：字符类别判断
来源：http://lin.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bqk.ctjpmb.com

[S22] C：字符串转数字
来源：http://imb.chenzaomai.com

atoi("42");  strtod("3.14", NULL);
来源：http://cfy.jiagoushi.top

[S23] C：随机数
来源：http://xiu.jinghuilouyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cad.smart0.xyz

[S24] C：获取本地时间
来源：http://tub.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wsa.pengpengdd.cyou

[S25] C：内存拷贝
来源：http://rsa.zhongyouzk.top

memcpy(dst, src, n);
来源：http://wsn.hnqzz.top

[S26] C：内存清零
来源：http://trv.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://bvg.chenlongwang.top

[S27] C：定义常量
来源：http://sfu.chenjidiqi.icu

const double PI = 3.14159;
来源：http://lqc.bjfxy.top

[S28] C：静态变量
来源：http://fkt.yongpay.top

static int counter = 0;
来源：http://gas.nanxuanxn.top

[S29] C：变参函数
来源：http://syz.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jmh.guannengcc.top

[S30] C：头文件保护
来源：http://oic.ivvv.top

#ifndef X_H
来源：http://gei.hnqzz.top

#define X_H
来源：http://oht.daxiang520.top

#endif
来源：http://pih.svipenyu.cn

[S31] C++：Hello World
来源：http://xsp.uphjek.com

#include <iostream>
来源：http://nxt.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://mxr.hnxiangtu.top

[S32] C++：字符串
来源：http://bdq.yonumen.top

std::string s = "hi";  s += "!";
来源：http://qsj.fengsongda.top

[S33] C++：vector 增删
来源：http://grz.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fbn.tanke756.top

[S34] C++：遍历 vector
来源：http://ujp.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://mqz.hammf.cn

[S35] C++：map
来源：http://bor.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gkg.epnwcf.com

[S36] C++：unordered_map
来源：http://ncv.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pnu.fehbvm.com

[S37] C++：set
来源：http://whx.gogol.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wou.jqgufenzy.top

[S38] C++：排序
来源：http://gom.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://jtc.yuanzhike.top


<!-- 参考信息 -->