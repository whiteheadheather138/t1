代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gkn.316326.xyz

[Q75] 日期格式化
来源：http://ugh.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://thl.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yyw.52xcode.cn

[Q76] 按天统计
来源：http://jnm.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vfh.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://dhs.haohaochexian.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ftk.fzhhl.top

[Q78] 当前时间
来源：http://wew.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bvt.hywenlv.cn

[Q79] 字符串拼接
来源：http://lom.meibo888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mrm.nanxinkj.top

[Q80] 字符串截取
来源：http://tbm.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bjz.9152youxi.cn

[Q81] 字符串替换
来源：http://knf.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uox.yj202588.top

[Q82] 字符长度与字节长度
来源：http://rve.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qrq.yonumen.top

[Q83] 大小写转换
来源：http://iuv.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fug.shzxlz.cn

[Q84] 去除首尾空格
来源：http://yxh.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://suc.hywenlv.cn

[Q85] 数值取整
来源：http://mpm.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gxr.hysaishi.cn

[Q86] 读取 JSON 字段
来源：http://nrw.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ikq.c1oappe.top

[Q87] JSON 字段做条件
来源：http://tjz.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vie.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://yhs.yangfankeji.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zpb.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qxj.nanxinkj.top

[Q89] 判断表是否存在
来源：http://jgp.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yzi.xziqi.cn

[Q90] 生成序号列
来源：http://vtg.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pxi.zhixingplan.top

================================================================================
来源：http://bzv.nanxinkj.top

R. Bash 专题
来源：http://ddp.yanxiufei.cn

================================================================================
来源：http://mpc.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://pvp.gotoacloud.top

#!/usr/bin/env bash
来源：http://zyk.fehbvm.com

set -euo pipefail
来源：http://yvp.0kj1m.cn

[R02] 变量赋值与使用
来源：http://hzk.cucudq.cn

name="Tom"; echo "$name"
来源：http://hnh.haohaochexian.top

[R03] 只读变量
来源：http://eve.haohaochexian.top

readonly PI=3.14
来源：http://dgh.shangyingyoupin.top

[R04] 位置参数
来源：http://vcu.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ppw.ydjk.org.cn

[R05] 参数默认值
来源：http://zua.bbcook.cn

name="${1:-default}"
来源：http://fuz.cheryme.top

[R06] 判断命令是否存在
来源：http://vjq.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ejl.guannengcc.top

[R07] if 判断文件
来源：http://dxr.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xfu.hnxiangtu.top

[R08] 数值比较
来源：http://osc.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bbh.ydzc1.top

[R09] 字符串比较
来源：http://hbi.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://abj.pengpengdd.cyou

[R10] 正则匹配
来源：http://kmd.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uny.iojbl.cn

[R11] case 多分支
来源：http://xom.dianchejie.cn

case "$1" in
来源：http://xtl.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://btm.ybcxt.top

stop)  echo "停止" ;;
来源：http://jfy.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://qur.yuxming.cn

esac
来源：http://lep.hnqzz.top

[R12] for 遍历文件
来源：http://ptr.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://czp.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://ieh.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://woc.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://xbw.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fbf.ivvv.top

[R15] while 逐行读文件
来源：http://gwu.hywenlv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uta.jinghuilouyu.cn

[R16] until 等待条件
来源：http://mqe.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rds.guowangkeji.top

[R17] 数组定义与取值
来源：http://kqz.vehdjk.com

arr=(a b c); echo "${arr[0]}"
来源：http://wgd.jinghuilouyu.cn

[R18] 遍历数组
来源：http://iti.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ksv.pycfn.com

[R19] 数组长度
来源：http://mcr.svipenyu.cn

echo "${#arr[@]}"
来源：http://ypm.haohaochexian.top

[R20] 关联数组（字典）
来源：http://ybg.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://slf.snrcjt.cn

[R21] 字符串长度
来源：http://muc.bbcook.cn

echo "${#s}"
来源：http://lue.hysaishi.cn

[R22] 截取子串
来源：http://cow.zhengqikj.top

echo "${s:0:5}"
来源：http://kdd.nanxuanxn.top

[R23] 字符串替换
来源：http://ulc.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jya.fktsv.cn

[R24] 大小写转换
来源：http://etd.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://ear.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://hhi.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://juj.jinqigufen.top

[R26] 命令替换
来源：http://zuw.shuidangran.top

now=$(date +%F); echo "$now"
来源：http://vde.fktsv.cn

[R27] 算术展开
来源：http://ucp.fktsv.cn

echo $((1 + 2 * 3))
来源：http://yil.yongpay.top

[R28] 浮点运算
来源：http://fee.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://gtc.0kj1m.cn

[R29] 定义函数
来源：http://tqp.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://png.daxiang520.top

[R30] 函数返回状态码
来源：http://ynn.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://qdp.chenzaomai.com

[R31] 局部变量
来源：http://pdw.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://kth.yonumen.top

[R32] 参数个数校验
来源：http://kdt.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gpn.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://juo.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fue.jlsjyb.cn

[R34] 退出时清理
来源：http://vge.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://afi.316326.xyz

[R35] 后台执行并等待
来源：http://tol.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://heu.yongpay.top

[R36] 并发执行多个任务
来源：http://qfa.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rqp.epnwcf.com

[R37] 把输出赋给变量
来源：http://tow.smart0.xyz

files=$(ls -1)
来源：http://bop.smart0.xyz

[R38] 管道串联
来源：http://vik.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://cib.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://dvl.jinqigufen.top

cmd > out.log 2>&1
来源：http://wcz.shangyingyoupin.top

[R40] 追加写日志
来源：http://cbu.daria6918.cn

echo "log" >> out.log
来源：http://dsu.yj20258.top

[R41] 丢弃输出
来源：http://iwe.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://cnp.jqgufenzy.top

[R42] 输入重定向
来源：http://uaj.hnxiangtu.top

wc -l < a.txt
来源：http://qed.aizwys.cn

[R43] 按名字查找文件
来源：http://gby.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://qjz.zycfv.cn

[R44] 按修改时间查找
来源：http://xec.vehdjk.com

find . -mtime -7 -type f
来源：http://rnj.ybcxt.top

[R45] 批量删除
来源：http://ccg.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://gsk.nanxinkj.top

[R46] 递归替换文件内容
来源：http://yyu.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rap.uphjek.com

[R47] sed 单行替换
来源：http://fmg.zdbjq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gru.yongpay.top

[R48] awk 取指定列
来源：http://krg.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://zqz.shangyingyoupin.top

[R49] awk 带条件
来源：http://ebo.guannengcc.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gga.feifeiyinyue.top

[R50] awk 求和
来源：http://odr.havefunace.top

awk '{s += $2} END {print s}' a.txt
来源：http://wyn.gaohongyu789.top

[R51] 排序去重取前几
来源：http://chk.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://cso.tanke756.top

[R52] 统计行数
来源：http://mfx.0kj1m.cn

wc -l a.txt
来源：http://tdp.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://dlg.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://amq.yueranfly.top

[R54] 比较两个文件
来源：http://hta.gogol.net.cn

diff a.txt b.txt
来源：http://trm.ydjk.org.cn

[R55] 压缩与解压
来源：http://weg.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://niv.zdqjudy.top

[R56] 远程拷贝
来源：http://ixq.haohaochexian.top

scp file user@host:/path/
来源：http://yqv.xziqi.cn

[R57] 远程执行命令
来源：http://egb.hcnkem.com

ssh user@host 'uptime'
来源：http://wzd.zhijiandao.cn

[R58] 下载文件
来源：http://nvq.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nmk.hcnkem.com

[R59] 发 POST JSON
来源：http://ysk.sjlbkw.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hnu.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://ptg.ivvv.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wkz.fengsongda.top

[R61] 磁盘占用
来源：http://yvb.zycfv.cn

df -h;  du -sh *
来源：http://qkq.yangfankeji.com

[R62] 找最占空间的文件
来源：http://vce.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://ltw.ydzc1.top

[R63] 内存与进程
来源：http://dnu.yj202588.top

free -h;  ps aux | grep nginx
来源：http://nzc.cashguo.top

[R64] 结束进程
来源：http://rvc.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://krj.gotoacloud.top

[R65] 查看端口占用
来源：http://jff.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ntb.shanyushiyangkeji.top

[R66] 定时任务
来源：http://ydm.daxiang520.top

crontab -e;  crontab -l
来源：http://pqc.shuidangran.top

[R67] 生成随机十六进制串
来源：http://lwa.havefunace.top

openssl rand -hex 16
来源：http://jnw.cdnleiting.top

[R68] 计算文件校验值
来源：http://nzg.jiagoushi.top

sha256sum a.txt;  md5sum a.txt
来源：http://ano.316326.xyz

[R69] 生成随机密码
来源：http://cim.hnxiangtu.top

head -c 16 /dev/urandom | base64
来源：http://ukk.jlsjyb.cn

[R70] 时间戳与互转
来源：http://ojt.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://aiu.yj202588.top

[R71] 日期格式化
来源：http://phr.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ynj.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://rws.sjlbkw.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gin.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://acc.ppjwa.cn

split -l 1000 big.log part_
来源：http://jfd.epnwcf.com

[R74] 批量重命名
来源：http://rkz.zhengqikj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cif.zhijiandao.cn

[R75] 导出环境变量
来源：http://dof.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://bzb.yj202588.top

[R76] 使用临时文件
来源：http://hbg.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hpo.chenzaomai.com

[R77] 读取用户输入
来源：http://cay.sweek.top

read -rp "请输入: " ans
来源：http://wyf.ehwqpu.com

[R78] 交互式菜单
来源：http://zsw.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://mmz.hammf.cn

[R79] 解析命令行选项
来源：http://yko.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vga.tarul.cn

[R80] 查看脚本执行耗时
来源：http://jgt.tarul.cn

time ./run.sh
来源：http://fdp.yuanzhike.top

================================================================================
来源：http://cgm.fehbvm.com

S. C / C++ 专题
来源：http://hhf.fktsv.cn

================================================================================
来源：http://qoa.redwolf501.top

[S01] C：Hello World
来源：http://gqv.jinqigfzy.top

#include <stdio.h>
来源：http://lnz.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ojv.hammf.cn

[S02] C：变量与格式化输出
来源：http://hiz.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://upz.jinghuilouyu.cn

[S03] C：读入整数
来源：http://rpp.fehbvm.com

int x; scanf("%d", &x);
来源：http://xfx.kuanghao11.cn

[S04] C：字符串复制
来源：http://ojb.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://ykz.svipenyu.cn

[S05] C：字符串长度
来源：http://xhp.sjlbkw.cn

strlen(s)
来源：http://usc.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://crw.gzhubu.top

strcmp(a, b) == 0
来源：http://mal.dashuyun.cn

[S07] C：数组遍历求和
来源：http://xbf.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rdm.yueranfly.top

[S08] C：动态内存分配与释放
来源：http://npo.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qkf.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://plz.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ojy.xylfe.cn

[S10] C：指针与解引用
来源：http://bhx.yvedp.cn

int *p = &a;  *p = 5;
来源：http://uex.quarkkingdee.top

[S11] C：逐行读文件
来源：http://csw.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://uhg.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oli.zhongyouzk.top

fclose(f);
来源：http://clh.chenzaomai.com

[S12] C：写文件
来源：http://kiw.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://trn.dianchejie.cn

[S13] C：宏定义
来源：http://eeb.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yla.gaohongyu789.top

[S14] C：枚举
来源：http://tdp.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://tav.ydjk.org.cn

[S15] C：类型转换
来源：http://iup.cdnleiting.top

(double) a / b
来源：http://ggn.zhijiandao.cn

[S16] C：位操作置位
来源：http://uns.fengsongda.top

x |= (1 << 3);
来源：http://uwo.fktsv.cn

[S17] C：安全拼接字符串
来源：http://pfc.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sfb.jqgufenzy.top

[S18] C：命令行参数
来源：http://vfk.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://xzo.ctjpmb.com

[S19] C：快速排序
来源：http://nsp.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ujw.smart0.xyz

[S20] C：二分查找
来源：http://lgu.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yuu.meibo888.top

[S21] C：字符类别判断
来源：http://hnl.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://htv.gaohongyu789.top

[S22] C：字符串转数字
来源：http://etk.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yzp.havefunace.top

[S23] C：随机数
来源：http://ktl.jqgfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bjq.meibo888.top

[S24] C：获取本地时间
来源：http://ese.hcnkem.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://quf.c1oappe.top

[S25] C：内存拷贝
来源：http://zek.yvedp.cn

memcpy(dst, src, n);
来源：http://aut.yj20258.top

[S26] C：内存清零
来源：http://uni.tian-w.cn

memset(a, 0, sizeof a);
来源：http://gix.mhx1999.top

[S27] C：定义常量
来源：http://sns.yfazqb.com

const double PI = 3.14159;
来源：http://crl.andypj.xyz

[S28] C：静态变量
来源：http://etv.hfpthk.cn

static int counter = 0;
来源：http://fcz.shuidangran.top

[S29] C：变参函数
来源：http://mix.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://elr.shanyushiyangtech.top

[S30] C：头文件保护
来源：http://zmi.ydzc1.top

#ifndef X_H
来源：http://gzw.svipenyu.cn

#define X_H
来源：http://ygk.xinyue.icu

#endif
来源：http://zfp.gaohongyu789.top

[S31] C++：Hello World
来源：http://pdi.guannengcc.top

#include <iostream>
来源：http://eac.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://huu.yanxiufei.cn

[S32] C++：字符串
来源：http://vlj.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://ogh.ydzc1.top

[S33] C++：vector 增删
来源：http://orn.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jkw.9152youxi.cn

[S34] C++：遍历 vector
来源：http://jom.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://drk.fktsv.cn

[S35] C++：map
来源：http://dvz.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://thj.shzxlz.cn

[S36] C++：unordered_map
来源：http://czj.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lue.gaohongyu789.top

[S37] C++：set
来源：http://utg.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://clk.smart0.xyz

[S38] C++：排序
来源：http://ryi.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://ljg.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://pog.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yny.jinghuilouyu.cn

[S40] C++：查找元素
来源：http://iue.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vdq.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://npa.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xwa.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://zco.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://urh.zhongyouzk.top

[S43] C++：智能指针
来源：http://xnn.haohaochexian.top

auto p = std::make_unique<int>(5);
来源：http://xnt.svipenyu.cn

[S44] C++：引用传参
来源：http://nhw.xinyue.icu

void inc(int &x) { ++x; }
来源：http://bzy.zhoulong.xyz


<!-- 参考信息 -->