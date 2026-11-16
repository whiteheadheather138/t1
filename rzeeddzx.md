代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ikz.ivvv.top

[Q75] 日期格式化
来源：http://gtb.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://twr.havefunace.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kgr.c1oappe.top

[Q76] 按天统计
来源：http://ovn.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lpn.fktsv.cn

[Q77] 时间加减
来源：http://kro.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qwt.mhx1999.top

[Q78] 当前时间
来源：http://btv.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ehw.xinyue.icu

[Q79] 字符串拼接
来源：http://kiz.guowangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fso.chenzaomai.com

[Q80] 字符串截取
来源：http://gwa.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xwv.yuanzhike.top

[Q81] 字符串替换
来源：http://rdg.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rwa.sxryk.cn

[Q82] 字符长度与字节长度
来源：http://yvm.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rnr.aizwys.cn

[Q83] 大小写转换
来源：http://uia.nanxuanxn.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bmy.zhiwuduotai.top

[Q84] 去除首尾空格
来源：http://ych.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://dyt.sjlbkw.cn

[Q85] 数值取整
来源：http://vch.jianghu66.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wyz.yonumen.top

[Q86] 读取 JSON 字段
来源：http://nht.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rbw.wangdashe.top

[Q87] JSON 字段做条件
来源：http://xej.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gdl.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://kvh.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xzx.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vxh.iojbl.cn

[Q89] 判断表是否存在
来源：http://bnx.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://via.kuanghao11.cn

[Q90] 生成序号列
来源：http://rac.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ezz.shzxlz.cn

================================================================================
来源：http://tjf.tanke756.top

R. Bash 专题
来源：http://xjd.jinqigfzy.top

================================================================================
来源：http://vec.daria6918.cn

[R01] shebang 与严格模式
来源：http://xyu.aibaodan.cn

#!/usr/bin/env bash
来源：http://mee.yj20258888.top

set -euo pipefail
来源：http://iaf.bjfxy.top

[R02] 变量赋值与使用
来源：http://hnl.haohaochexian.top

name="Tom"; echo "$name"
来源：http://mov.hongshengwenyu.top

[R03] 只读变量
来源：http://dni.tanke756.top

readonly PI=3.14
来源：http://miz.yongpay.top

[R04] 位置参数
来源：http://aka.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cda.cheryme.top

[R05] 参数默认值
来源：http://bxa.zhoulong.xyz

name="${1:-default}"
来源：http://qyr.meibo888.top

[R06] 判断命令是否存在
来源：http://sjc.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sdp.yuanzhike.top

[R07] if 判断文件
来源：http://lsj.jianghu66.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nll.yangfankeji.com

[R08] 数值比较
来源：http://jjg.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cdk.jinqigfzy.top

[R09] 字符串比较
来源：http://xpr.zhongyouzk.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xoa.redwolf501.top

[R10] 正则匹配
来源：http://lks.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eht.chenjidiqi.icu

[R11] case 多分支
来源：http://ldj.vqdsnc.cn

case "$1" in
来源：http://ftn.quarkkingdee.top

start) echo "启动" ;;
来源：http://opv.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://guz.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://klz.zhixingplan.top

esac
来源：http://xgt.316326.xyz

[R12] for 遍历文件
来源：http://exn.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://ftb.chenzaomai.com

[R13] for 计数循环
来源：http://xpi.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://ttc.fengsongda.top

[R14] C 风格 for
来源：http://oos.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eym.dianchejie.cn

[R15] while 逐行读文件
来源：http://rkb.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tiw.zhongyouzk.top

[R16] until 等待条件
来源：http://gjm.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dbo.snrcjt.cn

[R17] 数组定义与取值
来源：http://hix.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://xfy.fktsv.cn

[R18] 遍历数组
来源：http://xed.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uny.epnwcf.com

[R19] 数组长度
来源：http://lbf.tarul.cn

echo "${#arr[@]}"
来源：http://nvn.wangdashe.top

[R20] 关联数组（字典）
来源：http://qtr.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cdg.shanyushiyangkeji.top

[R21] 字符串长度
来源：http://qxx.zdbjq.cn

echo "${#s}"
来源：http://kuk.ehwqpu.com

[R22] 截取子串
来源：http://ybh.feifeiyinyue.top

echo "${s:0:5}"
来源：http://hny.52xcode.cn

[R23] 字符串替换
来源：http://wgc.guowangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pnp.uphjek.com

[R24] 大小写转换
来源：http://nqc.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://iqr.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://dky.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://xfv.redwolf501.top

[R26] 命令替换
来源：http://aaf.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://qpn.sweek.top

[R27] 算术展开
来源：http://eax.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://mol.mhx1999.top

[R28] 浮点运算
来源：http://gsb.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://kby.ppjwa.cn

[R29] 定义函数
来源：http://wjn.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ouj.c1oappe.top

[R30] 函数返回状态码
来源：http://ibi.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://vuz.tianlin.xyz

[R31] 局部变量
来源：http://nds.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://mie.ehwqpu.com

[R32] 参数个数校验
来源：http://xrb.shuidangran.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dyy.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://hxj.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gry.ybcxt.top

[R34] 退出时清理
来源：http://edd.yueranfly.top

trap 'rm -f "$tmp"' EXIT
来源：http://cns.yueranfly.top

[R35] 后台执行并等待
来源：http://smc.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rvu.shanyushiyangtech.top

[R36] 并发执行多个任务
来源：http://ygr.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nrm.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://kad.mhx1999.top

files=$(ls -1)
来源：http://hku.nanxuanxn.top

[R38] 管道串联
来源：http://zkt.jyoumei.cn

cat a.txt | grep -i error | wc -l
来源：http://cgm.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://pwd.ehwqpu.com

cmd > out.log 2>&1
来源：http://jzn.cheryme.top

[R40] 追加写日志
来源：http://mch.havefunace.top

echo "log" >> out.log
来源：http://ztp.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://ucg.xylfe.cn

cmd >/dev/null 2>&1
来源：http://tkd.cdnleiting.top

[R42] 输入重定向
来源：http://wxb.sjlbkw.cn

wc -l < a.txt
来源：http://lql.yvedp.cn

[R43] 按名字查找文件
来源：http://xfg.ctjpmb.com

find . -name "*.log" -type f
来源：http://sgf.fehbvm.com

[R44] 按修改时间查找
来源：http://tib.gotoacloud.top

find . -mtime -7 -type f
来源：http://nav.chenlongwang.top

[R45] 批量删除
来源：http://vkn.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://tzb.dashuyun.cn

[R46] 递归替换文件内容
来源：http://wqb.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xdl.smart0.xyz

[R47] sed 单行替换
来源：http://syh.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vom.yfazqb.com

[R48] awk 取指定列
来源：http://leg.zhaomingkeji.xyz

awk '{print $1, $3}' a.txt
来源：http://lae.chenlongwang.top

[R49] awk 带条件
来源：http://gbq.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mvx.jianghu66.top

[R50] awk 求和
来源：http://kim.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://ftg.ctjpmb.com

[R51] 排序去重取前几
来源：http://ruu.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ixh.daria6918.cn

[R52] 统计行数
来源：http://vqp.quarkkingdee.top

wc -l a.txt
来源：http://ndm.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://hlk.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://owr.jiagoushi.top

[R54] 比较两个文件
来源：http://iso.xziqi.cn

diff a.txt b.txt
来源：http://vdu.yj20258.top

[R55] 压缩与解压
来源：http://tfg.bbcook.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zzo.fktsv.cn

[R56] 远程拷贝
来源：http://kbf.yfazqb.com

scp file user@host:/path/
来源：http://dye.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://ujs.aizwys.cn

ssh user@host 'uptime'
来源：http://kgb.snrcjt.cn

[R58] 下载文件
来源：http://hvz.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://abu.tanke756.top

[R59] 发 POST JSON
来源：http://whv.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xmr.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://utq.ivvv.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ttn.zycfv.cn

[R61] 磁盘占用
来源：http://qxv.jinghuilouyu.cn

df -h;  du -sh *
来源：http://yag.52xcode.cn

[R62] 找最占空间的文件
来源：http://gul.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://vql.jlsjyb.cn

[R63] 内存与进程
来源：http://plt.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://rpu.hnxiangtu.top

[R64] 结束进程
来源：http://hai.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://sok.iojbl.cn

[R65] 查看端口占用
来源：http://qdg.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://msy.epnwcf.com

[R66] 定时任务
来源：http://lei.zhijiandao.cn

crontab -e;  crontab -l
来源：http://chm.xziqi.cn

[R67] 生成随机十六进制串
来源：http://cxd.fktsv.cn

openssl rand -hex 16
来源：http://nzx.shuidangran.top

[R68] 计算文件校验值
来源：http://yjx.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://kjx.fktsv.cn

[R69] 生成随机密码
来源：http://mkk.0kj1m.cn

head -c 16 /dev/urandom | base64
来源：http://vwx.cqqwz.cn

[R70] 时间戳与互转
来源：http://drk.xuanzx.com

date +%s;  date -d @1700000000
来源：http://yys.shangyingyoupin.top

[R71] 日期格式化
来源：http://ddu.guowangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cgi.ybcxt.top

[R72] 等待端口就绪
来源：http://bwe.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://spb.sjlbkw.cn

[R73] 分割大日志
来源：http://rap.gzhubu.top

split -l 1000 big.log part_
来源：http://sag.dianchejie.cn

[R74] 批量重命名
来源：http://pfv.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fnc.epnwcf.com

[R75] 导出环境变量
来源：http://tso.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://wuj.cucudq.cn

[R76] 使用临时文件
来源：http://top.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yrb.gzhubu.top

[R77] 读取用户输入
来源：http://fxq.gotoacloud.top

read -rp "请输入: " ans
来源：http://yjx.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://wji.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sxb.yanxiufei.cn

[R79] 解析命令行选项
来源：http://exl.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://azm.tarul.cn

[R80] 查看脚本执行耗时
来源：http://vfl.redwolf501.top

time ./run.sh
来源：http://gno.yj20258.top

================================================================================
来源：http://wka.tian-w.cn

S. C / C++ 专题
来源：http://xpe.gogol.net.cn

================================================================================
来源：http://dle.fzhhl.top

[S01] C：Hello World
来源：http://rfu.hnxiangtu.top

#include <stdio.h>
来源：http://vmn.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mbb.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://lee.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://pmp.aizwys.cn

[S03] C：读入整数
来源：http://vox.fengsongda.top

int x; scanf("%d", &x);
来源：http://wxh.mhx1999.top

[S04] C：字符串复制
来源：http://ouc.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jkk.dianchejie.cn

[S05] C：字符串长度
来源：http://dqv.daxiang520.top

strlen(s)
来源：http://klq.0kj1m.cn

[S06] C：字符串比较
来源：http://rfn.jinqigfzy.top

strcmp(a, b) == 0
来源：http://evm.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://aap.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ctp.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://etx.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://abh.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://hql.feifeiyinyue.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lte.kuanghao11.cn

[S10] C：指针与解引用
来源：http://deb.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://ggz.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://hcg.kuanghao11.cn

FILE *f = fopen("a.txt", "r");
来源：http://puh.zhixingplan.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://scq.bbcook.cn

fclose(f);
来源：http://hhm.hnxiangtu.top

[S12] C：写文件
来源：http://qec.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kix.fktsv.cn

[S13] C：宏定义
来源：http://dow.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wbs.sxryk.cn

[S14] C：枚举
来源：http://phn.zhoulong.xyz

enum Color { RED, GREEN, BLUE };
来源：http://gjj.nanxuanxn.top

[S15] C：类型转换
来源：http://lmn.shuidangran.top

(double) a / b
来源：http://azc.sjlbkw.cn

[S16] C：位操作置位
来源：http://kzr.yfazqb.com

x |= (1 << 3);
来源：http://ecr.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://ljm.xuanzx.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://syj.gaohongyu789.top

[S18] C：命令行参数
来源：http://ylw.shzxlz.cn

int main(int argc, char **argv)
来源：http://koc.sufxvd.cn

[S19] C：快速排序
来源：http://ikk.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://qqz.cdnleiting.top

[S20] C：二分查找
来源：http://hqe.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://drf.pycfn.com

[S21] C：字符类别判断
来源：http://qxk.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aal.zdqjudy.top

[S22] C：字符串转数字
来源：http://eki.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oyv.zhaomingkeji.xyz

[S23] C：随机数
来源：http://cur.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://urs.nwbrower.top

[S24] C：获取本地时间
来源：http://mep.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://amg.ybcxt.top

[S25] C：内存拷贝
来源：http://wqb.9152youxi.cn

memcpy(dst, src, n);
来源：http://gxq.zhongyouzk.top

[S26] C：内存清零
来源：http://dem.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://bsd.snrcjt.cn

[S27] C：定义常量
来源：http://mby.daxiang520.top

const double PI = 3.14159;
来源：http://idg.guowangkeji.top

[S28] C：静态变量
来源：http://jyj.shzxlz.cn

static int counter = 0;
来源：http://pyf.uphjek.com

[S29] C：变参函数
来源：http://qdn.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vaw.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://vrf.zycfv.cn

#ifndef X_H
来源：http://wip.cqqwz.cn

#define X_H
来源：http://oip.yangfankeji.com

#endif
来源：http://zbl.fktsv.cn

[S31] C++：Hello World
来源：http://tdr.cheryme.top

#include <iostream>
来源：http://nop.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://mrq.xuanzx.com

[S32] C++：字符串
来源：http://xxl.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://sqq.0kj1m.cn

[S33] C++：vector 增删
来源：http://pxu.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wxp.jiagoushi.top

[S34] C++：遍历 vector
来源：http://zlc.gogol.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://fzo.pengpengdd.cyou

[S35] C++：map
来源：http://tts.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jke.jiagoushi.top

[S36] C++：unordered_map
来源：http://jly.fzhhl.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ngi.ivvv.top

[S37] C++：set
来源：http://lph.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tzb.fanxiaobao.xyz

[S38] C++：排序
来源：http://mrq.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://zji.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://adu.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dji.xylfe.cn

[S40] C++：查找元素
来源：http://cqe.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://waa.daria6918.cn

[S41] C++：类与构造函数
来源：http://jsd.wangshuangyany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uhr.cucudq.cn

[S42] C++：继承与虚函数
来源：http://rnr.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://tnt.bjfxy.top

[S43] C++：智能指针
来源：http://fyc.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://xhz.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://nbg.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://qbb.shzxlz.cn


<!-- 参考信息 -->