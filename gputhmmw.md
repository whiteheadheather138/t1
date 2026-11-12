代发 wailian999

[Q76] 按天统计
来源：http://cxp.zdqjudy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ecu.yj20258.top

[Q77] 时间加减
来源：http://ccr.gotoacloud.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qqt.hywenlv.cn

[Q78] 当前时间
来源：http://fhq.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uru.hywenlv.cn

[Q79] 字符串拼接
来源：http://ery.mhx1999.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mhp.jinqigfzy.top

[Q80] 字符串截取
来源：http://azl.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gdy.fehbvm.com

[Q81] 字符串替换
来源：http://ade.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dxm.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://lgo.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uyy.fengsongda.top

[Q83] 大小写转换
来源：http://nle.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ojv.zhengqikj.top

[Q84] 去除首尾空格
来源：http://kbb.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://hgk.aibaodan.cn

[Q85] 数值取整
来源：http://jrp.zhiwuduotai.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zcj.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://sys.ywan-chungtsiang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nxl.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://znf.zhijiandao.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tmy.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://bwy.zhengqikj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nep.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xaq.gogol.net.cn

[Q89] 判断表是否存在
来源：http://rzx.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ggu.jqgufenzy.top

[Q90] 生成序号列
来源：http://iqh.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bqz.jianghu66.top

================================================================================
来源：http://fku.uphjek.com

R. Bash 专题
来源：http://thq.pycfn.com

================================================================================
来源：http://egx.jiagoushi.top

[R01] shebang 与严格模式
来源：http://uug.ehwqpu.com

#!/usr/bin/env bash
来源：http://vch.tanke756.top

set -euo pipefail
来源：http://fni.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://gpr.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://vau.zhongyouzk.top

[R03] 只读变量
来源：http://vfg.jinyuanbaomall.cn

readonly PI=3.14
来源：http://isa.jinyuanbaomall.cn

[R04] 位置参数
来源：http://mdx.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yxg.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://bgw.sweek.top

name="${1:-default}"
来源：http://wrj.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://gqg.zhaomingkeji.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yvy.zhijiandao.cn

[R07] if 判断文件
来源：http://tft.yj20258888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yhg.0kj1m.cn

[R08] 数值比较
来源：http://uhg.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wct.nanxuanxn.top

[R09] 字符串比较
来源：http://xcm.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kie.aibaodan.cn

[R10] 正则匹配
来源：http://fom.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jzx.yvedp.cn

[R11] case 多分支
来源：http://gvp.jinghuilouyu.cn

case "$1" in
来源：http://cko.yongpay.top

start) echo "启动" ;;
来源：http://fgc.dianchejie.cn

stop)  echo "停止" ;;
来源：http://tgc.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://wrc.yj20258.top

esac
来源：http://qxs.hongshengwenyu.top

[R12] for 遍历文件
来源：http://fmv.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://bkc.dashuyun.cn

[R13] for 计数循环
来源：http://khl.sufxvd.cn

for i in {1..10}; do echo "$i"; done
来源：http://luo.aizwys.cn

[R14] C 风格 for
来源：http://qwq.quarkkingdee.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jrg.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://igb.fanxiaobao.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ein.vehdjk.com

[R16] until 等待条件
来源：http://jch.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rwh.sufxvd.cn

[R17] 数组定义与取值
来源：http://inm.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://rrk.daria6918.cn

[R18] 遍历数组
来源：http://hmd.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zsf.ydzc1.top

[R19] 数组长度
来源：http://fyd.nwbrower.top

echo "${#arr[@]}"
来源：http://cyo.mhx1999.top

[R20] 关联数组（字典）
来源：http://kyr.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ros.pycfn.com

[R21] 字符串长度
来源：http://xnj.gogol.net.cn

echo "${#s}"
来源：http://igb.epnwcf.com

[R22] 截取子串
来源：http://xvb.tanke756.top

echo "${s:0:5}"
来源：http://eel.shanyushiyangtech.top

[R23] 字符串替换
来源：http://ohj.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mlk.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://yvw.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bfb.ydzc1.top

[R25] 去后缀 / 去前缀
来源：http://tmt.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ryz.redwolf501.top

[R26] 命令替换
来源：http://zga.jlsjyb.cn

now=$(date +%F); echo "$now"
来源：http://dtk.tian-w.cn

[R27] 算术展开
来源：http://kap.fzhhl.top

echo $((1 + 2 * 3))
来源：http://qds.316326.xyz

[R28] 浮点运算
来源：http://kzr.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://dcj.zhengqikj.top

[R29] 定义函数
来源：http://api.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qqt.hywenlv.cn

[R30] 函数返回状态码
来源：http://nea.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://xis.zhijiandao.cn

[R31] 局部变量
来源：http://qgw.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://dns.zhixingplan.top

[R32] 参数个数校验
来源：http://auo.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pxm.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://zei.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sgu.zhijiandao.cn

[R34] 退出时清理
来源：http://agc.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://qet.birdmap.top

[R35] 后台执行并等待
来源：http://tcx.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ubt.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://xhz.ivvv.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://myi.redwolf501.top

[R37] 把输出赋给变量
来源：http://qxo.yj20258888.top

files=$(ls -1)
来源：http://ukl.jqgufenzy.top

[R38] 管道串联
来源：http://bkl.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://njo.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://rqg.jinqigfzy.top

cmd > out.log 2>&1
来源：http://kiu.cheryme.top

[R40] 追加写日志
来源：http://fss.xziqi.cn

echo "log" >> out.log
来源：http://kvq.aizwys.cn

[R41] 丢弃输出
来源：http://lwj.yj202588.top

cmd >/dev/null 2>&1
来源：http://ygj.zhixingplan.top

[R42] 输入重定向
来源：http://tvc.nwbrower.top

wc -l < a.txt
来源：http://ltc.jinqigfzy.top

[R43] 按名字查找文件
来源：http://gww.ydzc1.top

find . -name "*.log" -type f
来源：http://frt.epnwcf.com

[R44] 按修改时间查找
来源：http://zgj.zycfv.cn

find . -mtime -7 -type f
来源：http://ask.yonumen.top

[R45] 批量删除
来源：http://jvo.xuanzx.com

find . -name "*.tmp" -delete
来源：http://dfy.birdmap.top

[R46] 递归替换文件内容
来源：http://pjh.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ozx.wangshuangyany.cn

[R47] sed 单行替换
来源：http://vkr.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fla.hesvh.cn

[R48] awk 取指定列
来源：http://ybh.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://hmj.yonumen.top

[R49] awk 带条件
来源：http://qmw.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://thw.jinghuilouyu.cn

[R50] awk 求和
来源：http://evz.wangdashe.top

awk '{s += $2} END {print s}' a.txt
来源：http://dmb.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://ser.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kko.zdqjudy.top

[R52] 统计行数
来源：http://jpd.zhixingplan.top

wc -l a.txt
来源：http://dfj.birdmap.top

[R53] 查看文件头与实时尾
来源：http://rfg.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://liz.chenlongwang.top

[R54] 比较两个文件
来源：http://frb.hywenlv.cn

diff a.txt b.txt
来源：http://rpk.tarul.cn

[R55] 压缩与解压
来源：http://ovk.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kax.jianghu66.top

[R56] 远程拷贝
来源：http://sad.zycfv.cn

scp file user@host:/path/
来源：http://vqy.sweek.top

[R57] 远程执行命令
来源：http://pgl.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://aij.havefunace.top

[R58] 下载文件
来源：http://udv.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gwf.yvedp.cn

[R59] 发 POST JSON
来源：http://zbk.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gyz.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://buu.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xan.feifeiyinyue.top

[R61] 磁盘占用
来源：http://rks.yj20258.top

df -h;  du -sh *
来源：http://crp.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://ctb.andypj.xyz

du -ah . | sort -rh | head -10
来源：http://umk.fktsv.cn

[R63] 内存与进程
来源：http://vcy.shanyushiyangtech.top

free -h;  ps aux | grep nginx
来源：http://rpg.epnwcf.com

[R64] 结束进程
来源：http://nsi.redwolf501.top

kill -9 $(pgrep -f app.py)
来源：http://mcp.meibo888.top

[R65] 查看端口占用
来源：http://enq.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://glp.hnxiangtu.top

[R66] 定时任务
来源：http://jkg.jlsjyb.cn

crontab -e;  crontab -l
来源：http://qnl.zhengqikj.top

[R67] 生成随机十六进制串
来源：http://grc.tian-w.cn

openssl rand -hex 16
来源：http://bfh.hnxiangtu.top

[R68] 计算文件校验值
来源：http://bop.zhengqikj.top

sha256sum a.txt;  md5sum a.txt
来源：http://fcu.yj202588.top

[R69] 生成随机密码
来源：http://lfq.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://iwr.ydzc1.top

[R70] 时间戳与互转
来源：http://eoe.xylfe.cn

date +%s;  date -d @1700000000
来源：http://xuz.svipenyu.cn

[R71] 日期格式化
来源：http://bco.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ksu.quarkkingdee.top

[R72] 等待端口就绪
来源：http://hnj.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oar.zhiwuduotai.top

[R73] 分割大日志
来源：http://xxy.sysykeji.top

split -l 1000 big.log part_
来源：http://fvw.cqqwz.cn

[R74] 批量重命名
来源：http://vde.ywan-chungtsiang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uww.yfazqb.com

[R75] 导出环境变量
来源：http://vqe.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://rfd.epnwcf.com

[R76] 使用临时文件
来源：http://cld.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ots.zhiwuduotai.top

[R77] 读取用户输入
来源：http://vts.jianghu66.top

read -rp "请输入: " ans
来源：http://kdx.xuetiantiany.cn

[R78] 交互式菜单
来源：http://wta.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jqb.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://wcb.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uvp.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://bkg.xinyue.icu

time ./run.sh
来源：http://hph.ydjk.org.cn

================================================================================
来源：http://rdi.tarul.cn

S. C / C++ 专题
来源：http://ucd.vehdjk.com

================================================================================
来源：http://jnf.jinghuilouyu.cn

[S01] C：Hello World
来源：http://grq.gotoacloud.top

#include <stdio.h>
来源：http://kxd.sxryk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gxh.daxiang520.top

[S02] C：变量与格式化输出
来源：http://nfu.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://gre.yuanzhike.top

[S03] C：读入整数
来源：http://sdf.ybcxt.top

int x; scanf("%d", &x);
来源：http://epv.zhiwuduotai.top

[S04] C：字符串复制
来源：http://kvs.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://ozb.gotoacloud.top

[S05] C：字符串长度
来源：http://jeg.hywenlv.cn

strlen(s)
来源：http://xfw.sysykeji.top

[S06] C：字符串比较
来源：http://chg.daxiang520.top

strcmp(a, b) == 0
来源：http://egw.fktsv.cn

[S07] C：数组遍历求和
来源：http://eex.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://imc.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://tam.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bxp.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://edz.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hgy.wangdashe.top

[S10] C：指针与解引用
来源：http://cju.epnwcf.com

int *p = &a;  *p = 5;
来源：http://bvc.yj202588.top

[S11] C：逐行读文件
来源：http://jrz.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://gqq.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vsr.cdnleiting.top

fclose(f);
来源：http://yht.yfazqb.com

[S12] C：写文件
来源：http://doa.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mmk.zhijiandao.cn

[S13] C：宏定义
来源：http://pme.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qxi.birdmap.top

[S14] C：枚举
来源：http://kau.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://qib.cdnleiting.top

[S15] C：类型转换
来源：http://smc.chenlongwang.top

(double) a / b
来源：http://sgn.uphjek.com

[S16] C：位操作置位
来源：http://vei.316326.xyz

x |= (1 << 3);
来源：http://wpv.cashguo.top

[S17] C：安全拼接字符串
来源：http://yhb.aibaodan.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hsq.fengsongda.top

[S18] C：命令行参数
来源：http://mvo.hnxiangtu.top

int main(int argc, char **argv)
来源：http://sxx.jqgfzy.top

[S19] C：快速排序
来源：http://pco.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://gzi.guannengcc.top

[S20] C：二分查找
来源：http://dwm.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qrg.ydzc1.top

[S21] C：字符类别判断
来源：http://mos.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://arw.yangfankeji.com

[S22] C：字符串转数字
来源：http://mlz.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://zro.chenlongwang.top

[S23] C：随机数
来源：http://lhs.shuidangran.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bbs.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://syy.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hwo.yuanzhike.top

[S25] C：内存拷贝
来源：http://mzv.fzhhl.top

memcpy(dst, src, n);
来源：http://syt.wangshuangyany.cn

[S26] C：内存清零
来源：http://eil.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://otp.cheryme.top

[S27] C：定义常量
来源：http://fuh.mhx1999.top

const double PI = 3.14159;
来源：http://sqf.jinqigufen.top

[S28] C：静态变量
来源：http://lmv.ivvv.top

static int counter = 0;
来源：http://dzv.cdnleiting.top

[S29] C：变参函数
来源：http://piv.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qxx.uphjek.com

[S30] C：头文件保护
来源：http://xem.chenlongwang.top

#ifndef X_H
来源：http://twh.hammf.cn

#define X_H
来源：http://iwz.cheryme.top

#endif
来源：http://dnz.havefunace.top

[S31] C++：Hello World
来源：http://udu.yangfankeji.com

#include <iostream>
来源：http://bzu.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://zio.yj20258.top

[S32] C++：字符串
来源：http://xrs.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://jas.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://cyt.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://teo.c1oappe.top

[S34] C++：遍历 vector
来源：http://wlq.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://twe.yueranfly.top

[S35] C++：map
来源：http://uez.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qun.hammf.cn

[S36] C++：unordered_map
来源：http://ovw.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ean.shanyushiyangkeji.top

[S37] C++：set
来源：http://iug.havefunace.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rah.0kj1m.cn

[S38] C++：排序
来源：http://zzt.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://mrd.zhengqikj.top

[S39] C++：自定义比较器排序
来源：http://ukz.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nxb.yj202588.top

[S40] C++：查找元素
来源：http://qto.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kev.ppjwa.cn

[S41] C++：类与构造函数
来源：http://zex.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://apj.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://duk.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://mtd.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://iqg.jinqigfzy.top

auto p = std::make_unique<int>(5);
来源：http://nhk.redwolf501.top

[S44] C++：引用传参
来源：http://yjr.hcnkem.com

void inc(int &x) { ++x; }
来源：http://xbl.ehwqpu.com

[S45] C++：lambda
来源：http://poa.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ury.snrcjt.cn

[S46] C++：函数模板
来源：http://unp.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jas.gzhubu.top


<!-- 参考信息 -->