代发 wailian999

[Q78] 当前时间
来源：http://boq.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tus.cashguo.top

[Q79] 字符串拼接
来源：http://mng.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xar.tianlin.xyz

[Q80] 字符串截取
来源：http://rys.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gdm.aibaodan.cn

[Q81] 字符串替换
来源：http://ahz.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xam.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://wyg.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dme.wangshuangyany.cn

[Q83] 大小写转换
来源：http://nyn.meibo888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eig.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://jkl.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://uck.iojbl.cn

[Q85] 数值取整
来源：http://zie.316326.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eki.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://and.shanyushiyangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wpj.xinyue.icu

[Q87] JSON 字段做条件
来源：http://htr.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tpo.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://dky.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ayg.52xcode.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ybz.sxryk.cn

[Q89] 判断表是否存在
来源：http://xgk.fzhhl.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uak.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://xfu.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wrb.guowangkeji.top

================================================================================
来源：http://vey.gaohongyu789.top

R. Bash 专题
来源：http://fmy.316326.xyz

================================================================================
来源：http://vco.daria6918.cn

[R01] shebang 与严格模式
来源：http://sjc.yongpay.top

#!/usr/bin/env bash
来源：http://tpe.nanxuanxn.top

set -euo pipefail
来源：http://rod.vqdsnc.cn

[R02] 变量赋值与使用
来源：http://vsm.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://yoj.c1oappe.top

[R03] 只读变量
来源：http://dyz.epnwcf.com

readonly PI=3.14
来源：http://dlt.yonumen.top

[R04] 位置参数
来源：http://xyn.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gsu.yvedp.cn

[R05] 参数默认值
来源：http://ote.316326.xyz

name="${1:-default}"
来源：http://asz.sweek.top

[R06] 判断命令是否存在
来源：http://xqw.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nlk.ydzc1.top

[R07] if 判断文件
来源：http://spp.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cmu.dianchejie.cn

[R08] 数值比较
来源：http://jya.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pit.zhoulong.xyz

[R09] 字符串比较
来源：http://utn.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nxp.guowangkeji.top

[R10] 正则匹配
来源：http://szo.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://esy.ydzc1.top

[R11] case 多分支
来源：http://nxu.ybcxt.top

case "$1" in
来源：http://xod.hongshengwenyu.top

start) echo "启动" ;;
来源：http://fsz.hywenlv.cn

stop)  echo "停止" ;;
来源：http://dqn.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://boh.chenjidiqi.icu

esac
来源：http://vfy.vehdjk.com

[R12] for 遍历文件
来源：http://pjf.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://ita.snrcjt.cn

[R13] for 计数循环
来源：http://zbr.sjlbkw.cn

for i in {1..10}; do echo "$i"; done
来源：http://yip.nanxuanxn.top

[R14] C 风格 for
来源：http://xvb.zhengqikj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://slb.redwolf501.top

[R15] while 逐行读文件
来源：http://dhd.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iyc.tarul.cn

[R16] until 等待条件
来源：http://yyp.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://koq.zdqjudy.top

[R17] 数组定义与取值
来源：http://lzn.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://kno.yanxiufei.cn

[R18] 遍历数组
来源：http://ern.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ntx.sysykeji.top

[R19] 数组长度
来源：http://wcx.sufxvd.cn

echo "${#arr[@]}"
来源：http://fsz.hnqzz.top

[R20] 关联数组（字典）
来源：http://olu.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bro.hesvh.cn

[R21] 字符串长度
来源：http://oqh.gotoacloud.top

echo "${#s}"
来源：http://rto.cashguo.top

[R22] 截取子串
来源：http://rcz.hfpthk.cn

echo "${s:0:5}"
来源：http://jep.yanxiufei.cn

[R23] 字符串替换
来源：http://wdd.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hbz.xuanzx.com

[R24] 大小写转换
来源：http://mur.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://fhw.wangshuangyany.cn

[R25] 去后缀 / 去前缀
来源：http://lgs.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://jxj.svipenyu.cn

[R26] 命令替换
来源：http://lup.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://vhb.fehbvm.com

[R27] 算术展开
来源：http://enj.smart0.xyz

echo $((1 + 2 * 3))
来源：http://vab.ydzc1.top

[R28] 浮点运算
来源：http://xav.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://rdc.jiagoushi.top

[R29] 定义函数
来源：http://egx.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pvf.tianlin.xyz

[R30] 函数返回状态码
来源：http://vpc.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://iuh.nwbrower.top

[R31] 局部变量
来源：http://ksc.ppjwa.cn

f() { local x=1; echo "$x"; }
来源：http://gwy.havefunace.top

[R32] 参数个数校验
来源：http://tgy.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cub.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://qwd.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rhc.jianghu66.top

[R34] 退出时清理
来源：http://xsi.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://ntn.jqgfzy.top

[R35] 后台执行并等待
来源：http://waz.ehwqpu.com

sleep 5 & pid=$!; wait "$pid"
来源：http://owh.yuanzhike.top

[R36] 并发执行多个任务
来源：http://rbj.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bxd.haohaochexian.top

[R37] 把输出赋给变量
来源：http://lun.gaohongyu789.top

files=$(ls -1)
来源：http://ycu.sjlbkw.cn

[R38] 管道串联
来源：http://xmm.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://att.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://mce.tanke756.top

cmd > out.log 2>&1
来源：http://tma.cashguo.top

[R40] 追加写日志
来源：http://mxx.c1oappe.top

echo "log" >> out.log
来源：http://fni.tian-w.cn

[R41] 丢弃输出
来源：http://mge.yj20258.top

cmd >/dev/null 2>&1
来源：http://pqs.c1oappe.top

[R42] 输入重定向
来源：http://fba.meibo888.top

wc -l < a.txt
来源：http://kwm.vehdjk.com

[R43] 按名字查找文件
来源：http://osh.gotoacloud.top

find . -name "*.log" -type f
来源：http://ygm.fzhhl.top

[R44] 按修改时间查找
来源：http://oxx.sxryk.cn

find . -mtime -7 -type f
来源：http://gxo.yvedp.cn

[R45] 批量删除
来源：http://ptw.yj20258.top

find . -name "*.tmp" -delete
来源：http://xvq.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://yln.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cnu.shuidangran.top

[R47] sed 单行替换
来源：http://gjm.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://zcg.gaohongyu789.top

[R48] awk 取指定列
来源：http://lju.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://efu.ydzc1.top

[R49] awk 带条件
来源：http://qaj.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dhi.birdmap.top

[R50] awk 求和
来源：http://mqv.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sjl.ydjk.org.cn

[R51] 排序去重取前几
来源：http://dth.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rik.dashuyun.cn

[R52] 统计行数
来源：http://jvk.yj202588.top

wc -l a.txt
来源：http://pjv.guowangkeji.top

[R53] 查看文件头与实时尾
来源：http://jpy.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hxa.sjlbkw.cn

[R54] 比较两个文件
来源：http://mxd.snrcjt.cn

diff a.txt b.txt
来源：http://sdh.hnxiangtu.top

[R55] 压缩与解压
来源：http://ada.zhixingplan.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ryb.ppjwa.cn

[R56] 远程拷贝
来源：http://ruo.yj20258888.top

scp file user@host:/path/
来源：http://hpr.iojbl.cn

[R57] 远程执行命令
来源：http://tos.svipenyu.cn

ssh user@host 'uptime'
来源：http://rsy.zhengqikj.top

[R58] 下载文件
来源：http://bcq.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bxm.shanyushiyangkeji.top

[R59] 发 POST JSON
来源：http://tsk.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zsz.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://igx.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vte.kuanghao11.cn

[R61] 磁盘占用
来源：http://vvs.fanxiaobao.xyz

df -h;  du -sh *
来源：http://lqy.cdnleiting.top

[R62] 找最占空间的文件
来源：http://azl.jinghuilouyu.cn

du -ah . | sort -rh | head -10
来源：http://rtc.nwbrower.top

[R63] 内存与进程
来源：http://gae.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://vvz.zhixingplan.top

[R64] 结束进程
来源：http://agt.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://wox.zhongyouzk.top

[R65] 查看端口占用
来源：http://tzu.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rnh.fktsv.cn

[R66] 定时任务
来源：http://vic.yuanzhike.top

crontab -e;  crontab -l
来源：http://jyz.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://swd.9152youxi.cn

openssl rand -hex 16
来源：http://gdl.yuanzhike.top

[R68] 计算文件校验值
来源：http://tvl.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://rsv.zhoulong.xyz

[R69] 生成随机密码
来源：http://xdi.jyoumei.cn

head -c 16 /dev/urandom | base64
来源：http://luc.jiagoushi.top

[R70] 时间戳与互转
来源：http://ocu.yvedp.cn

date +%s;  date -d @1700000000
来源：http://aeo.hnqzz.top

[R71] 日期格式化
来源：http://bzh.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qwn.sjlbkw.cn

[R72] 等待端口就绪
来源：http://hwo.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eln.fengsongda.top

[R73] 分割大日志
来源：http://xxq.zhengqikj.top

split -l 1000 big.log part_
来源：http://yae.gotoacloud.top

[R74] 批量重命名
来源：http://fje.jqgfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ppg.aibaodan.cn

[R75] 导出环境变量
来源：http://oub.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://zmi.ppjwa.cn

[R76] 使用临时文件
来源：http://oym.guowangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://drp.sxryk.cn

[R77] 读取用户输入
来源：http://qxz.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://tdt.jiagoushi.top

[R78] 交互式菜单
来源：http://xhl.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hoq.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://dag.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://voc.zdqjudy.top

[R80] 查看脚本执行耗时
来源：http://lss.shzxlz.cn

time ./run.sh
来源：http://irc.kuanghao11.cn

================================================================================
来源：http://hbc.pengpengdd.cyou

S. C / C++ 专题
来源：http://wbv.hysaishi.cn

================================================================================
来源：http://usd.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://piq.vehdjk.com

#include <stdio.h>
来源：http://qvm.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://emt.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://vpo.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://cmw.bjfxy.top

[S03] C：读入整数
来源：http://pyc.sweek.top

int x; scanf("%d", &x);
来源：http://ang.shzxlz.cn

[S04] C：字符串复制
来源：http://tsi.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://qnf.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://ejb.tianlin.xyz

strlen(s)
来源：http://qnr.jinqigufen.top

[S06] C：字符串比较
来源：http://pub.zdbjq.cn

strcmp(a, b) == 0
来源：http://ett.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://tbt.ywan-chungtsiang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qmt.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://rjc.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gbb.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://guu.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ezs.hcnkem.com

[S10] C：指针与解引用
来源：http://vlg.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://jmk.yfazqb.com

[S11] C：逐行读文件
来源：http://mev.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://aou.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://guo.yj20258.top

fclose(f);
来源：http://fkn.vqdsnc.cn

[S12] C：写文件
来源：http://dbo.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zba.chenjidiqi.icu

[S13] C：宏定义
来源：http://iaz.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oib.sxryk.cn

[S14] C：枚举
来源：http://aes.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://hak.ydjk.org.cn

[S15] C：类型转换
来源：http://pib.sysykeji.top

(double) a / b
来源：http://cxc.hesvh.cn

[S16] C：位操作置位
来源：http://lvb.wangdashe.top

x |= (1 << 3);
来源：http://iyx.bjfxy.top

[S17] C：安全拼接字符串
来源：http://tls.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ghy.ybcxt.top

[S18] C：命令行参数
来源：http://qvl.xziqi.cn

int main(int argc, char **argv)
来源：http://xpn.yj20258888.top

[S19] C：快速排序
来源：http://rky.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://eys.cdnleiting.top

[S20] C：二分查找
来源：http://ylz.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ipp.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://zew.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nch.gogol.net.cn

[S22] C：字符串转数字
来源：http://dbv.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://apl.yvedp.cn

[S23] C：随机数
来源：http://dfa.gogol.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://biy.nwbrower.top

[S24] C：获取本地时间
来源：http://qel.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vtl.birdmap.top

[S25] C：内存拷贝
来源：http://ltp.birdmap.top

memcpy(dst, src, n);
来源：http://cvo.zdbjq.cn

[S26] C：内存清零
来源：http://bcc.yonumen.top

memset(a, 0, sizeof a);
来源：http://elw.quarkkingdee.top

[S27] C：定义常量
来源：http://rup.guannengcc.top

const double PI = 3.14159;
来源：http://yxq.ydjk.org.cn

[S28] C：静态变量
来源：http://zvy.uphjek.com

static int counter = 0;
来源：http://tgu.fengsongda.top

[S29] C：变参函数
来源：http://oii.yvedp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kxt.jinqigfzy.top

[S30] C：头文件保护
来源：http://mpw.zycfv.cn

#ifndef X_H
来源：http://gxc.dashuyun.cn

#define X_H
来源：http://nno.yongpay.top

#endif
来源：http://lao.gotoacloud.top

[S31] C++：Hello World
来源：http://sos.hongshengwenyu.top

#include <iostream>
来源：http://etn.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://spk.zhijiandao.cn

[S32] C++：字符串
来源：http://jgi.yongpay.top

std::string s = "hi";  s += "!";
来源：http://qex.cashguo.top

[S33] C++：vector 增删
来源：http://bss.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eek.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://vby.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://zna.jinyuanbaomall.cn

[S35] C++：map
来源：http://jag.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://knz.yj20258888.top

[S36] C++：unordered_map
来源：http://jev.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hqz.hongshengwenyu.top

[S37] C++：set
来源：http://khe.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kth.zhengqikj.top

[S38] C++：排序
来源：http://zxy.shanyushiyangkeji.top

std::sort(v.begin(), v.end());
来源：http://nsb.sufxvd.cn

[S39] C++：自定义比较器排序
来源：http://nns.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ecm.jqgfzy.top

[S40] C++：查找元素
来源：http://lmg.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nkk.9152youxi.cn

[S41] C++：类与构造函数
来源：http://dvu.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rpf.tarul.cn

[S42] C++：继承与虚函数
来源：http://ojq.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://ovt.hongshengwenyu.top

[S43] C++：智能指针
来源：http://zzw.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://enl.fengsongda.top

[S44] C++：引用传参
来源：http://cxw.fzhhl.top

void inc(int &x) { ++x; }
来源：http://egr.tianlin.xyz

[S45] C++：lambda
来源：http://xrs.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://mhu.dashuyun.cn

[S46] C++：函数模板
来源：http://vfw.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wcp.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://umy.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ujo.hesvh.cn

[S48] C++：逐行读文件
来源：http://bcz.gotoacloud.top

std::ifstream in("a.txt");  std::string line;
来源：http://sej.xinyue.icu


<!-- 参考信息 -->