代发 wailian999

[Q78] 当前时间
来源：http://eyg.zdqjudy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aqx.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://zyc.jinghuilouyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ozu.hcnkem.com

[Q80] 字符串截取
来源：http://mrc.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zqv.guowangkeji.top

[Q81] 字符串替换
来源：http://fnp.hywenlv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://psv.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://ltb.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://auv.aizwys.cn

[Q83] 大小写转换
来源：http://ozj.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tpf.redwolf501.top

[Q84] 去除首尾空格
来源：http://wij.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://apn.havefunace.top

[Q85] 数值取整
来源：http://wem.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bho.jianghu66.top

[Q86] 读取 JSON 字段
来源：http://jpb.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jpl.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://vfa.ehwqpu.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vdd.yfazqb.com

[Q88] 行转列（条件聚合）
来源：http://xja.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://idm.sufxvd.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xfj.tian-w.cn

[Q89] 判断表是否存在
来源：http://qmt.yfazqb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ljl.gotoacloud.top

[Q90] 生成序号列
来源：http://goj.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://igm.chenlongwang.top

================================================================================
来源：http://jfv.sweek.top

R. Bash 专题
来源：http://kyc.uphjek.com

================================================================================
来源：http://pim.tanke756.top

[R01] shebang 与严格模式
来源：http://oxk.ydzc1.top

#!/usr/bin/env bash
来源：http://nop.shuidangran.top

set -euo pipefail
来源：http://kjp.daxiang520.top

[R02] 变量赋值与使用
来源：http://qqp.fktsv.cn

name="Tom"; echo "$name"
来源：http://iir.zhongyouzk.top

[R03] 只读变量
来源：http://gzu.nanxinkj.top

readonly PI=3.14
来源：http://rpp.sysykeji.top

[R04] 位置参数
来源：http://gbw.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rds.zdqjudy.top

[R05] 参数默认值
来源：http://tms.dashuyun.cn

name="${1:-default}"
来源：http://ahx.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://syk.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fqj.yfazqb.com

[R07] if 判断文件
来源：http://bua.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wal.hongshengwenyu.top

[R08] 数值比较
来源：http://yav.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hgy.gaohongyu789.top

[R09] 字符串比较
来源：http://cyo.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hvd.sysykeji.top

[R10] 正则匹配
来源：http://qzj.tian-w.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vkv.aizwys.cn

[R11] case 多分支
来源：http://sqi.xinyue.icu

case "$1" in
来源：http://tmp.yj20258888.top

start) echo "启动" ;;
来源：http://kak.sweek.top

stop)  echo "停止" ;;
来源：http://fkw.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://yds.sweek.top

esac
来源：http://aji.shuidangran.top

[R12] for 遍历文件
来源：http://che.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://cul.gaohongyu789.top

[R13] for 计数循环
来源：http://pic.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://cty.52xcode.cn

[R14] C 风格 for
来源：http://ckw.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://unz.52xcode.cn

[R15] while 逐行读文件
来源：http://gcc.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xih.hnqzz.top

[R16] until 等待条件
来源：http://dld.aibaodan.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zmh.kuanghao11.cn

[R17] 数组定义与取值
来源：http://zpt.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://riu.hnqzz.top

[R18] 遍历数组
来源：http://hrw.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mkf.aizwys.cn

[R19] 数组长度
来源：http://tzn.c1oappe.top

echo "${#arr[@]}"
来源：http://ubz.52xcode.cn

[R20] 关联数组（字典）
来源：http://qfn.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wxg.mhx1999.top

[R21] 字符串长度
来源：http://nka.sysykeji.top

echo "${#s}"
来源：http://ood.sjlbkw.cn

[R22] 截取子串
来源：http://dau.xuanzx.com

echo "${s:0:5}"
来源：http://ens.nanxinkj.top

[R23] 字符串替换
来源：http://kxp.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bku.zycfv.cn

[R24] 大小写转换
来源：http://ypb.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://qxd.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://eib.ctjpmb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://iza.ydjk.org.cn

[R26] 命令替换
来源：http://dbt.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://sxo.cucudq.cn

[R27] 算术展开
来源：http://pjs.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://lix.yj202588.top

[R28] 浮点运算
来源：http://inr.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://tok.ybcxt.top

[R29] 定义函数
来源：http://jld.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vuw.jinqigufen.top

[R30] 函数返回状态码
来源：http://qqg.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://sot.xuanzx.com

[R31] 局部变量
来源：http://lsx.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://gtg.sysykeji.top

[R32] 参数个数校验
来源：http://cwy.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xpv.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://jai.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fuo.cqqwz.cn

[R34] 退出时清理
来源：http://aqf.nwbrower.top

trap 'rm -f "$tmp"' EXIT
来源：http://umi.epnwcf.com

[R35] 后台执行并等待
来源：http://hdp.wangdashe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://swo.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://dio.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nih.hnqzz.top

[R37] 把输出赋给变量
来源：http://thd.yj202588.top

files=$(ls -1)
来源：http://vsk.zhixingplan.top

[R38] 管道串联
来源：http://gqi.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://sdz.yonumen.top

[R39] 重定向标准输出与错误
来源：http://nfn.sufxvd.cn

cmd > out.log 2>&1
来源：http://pzj.tian-w.cn

[R40] 追加写日志
来源：http://ynf.tianlin.xyz

echo "log" >> out.log
来源：http://tbn.jqgfzy.top

[R41] 丢弃输出
来源：http://mle.yuxming.cn

cmd >/dev/null 2>&1
来源：http://nby.jinyuanbaomall.cn

[R42] 输入重定向
来源：http://sat.fengsongda.top

wc -l < a.txt
来源：http://msf.zhijiandao.cn

[R43] 按名字查找文件
来源：http://yin.ydzc1.top

find . -name "*.log" -type f
来源：http://yvh.sxryk.cn

[R44] 按修改时间查找
来源：http://qah.ybcxt.top

find . -mtime -7 -type f
来源：http://rgh.tian-w.cn

[R45] 批量删除
来源：http://uns.daria6918.cn

find . -name "*.tmp" -delete
来源：http://cqu.c1oappe.top

[R46] 递归替换文件内容
来源：http://vue.xuanzx.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dij.sweek.top

[R47] sed 单行替换
来源：http://jer.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://cgs.xuanzx.com

[R48] awk 取指定列
来源：http://gfk.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://ovd.nanxinkj.top

[R49] awk 带条件
来源：http://vwu.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lsy.xziqi.cn

[R50] awk 求和
来源：http://upu.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://ffv.jianghu66.top

[R51] 排序去重取前几
来源：http://sjn.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ivz.aibaodan.cn

[R52] 统计行数
来源：http://sgc.quarkkingdee.top

wc -l a.txt
来源：http://gze.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://igz.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qfs.guowangkeji.top

[R54] 比较两个文件
来源：http://hvk.jinqigfzy.top

diff a.txt b.txt
来源：http://rmg.ydzc1.top

[R55] 压缩与解压
来源：http://uqi.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://duq.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://vwd.sweek.top

scp file user@host:/path/
来源：http://rnm.jqgufenzy.top

[R57] 远程执行命令
来源：http://lod.ywan-chungtsiang.top

ssh user@host 'uptime'
来源：http://wgj.xuanzx.com

[R58] 下载文件
来源：http://dfg.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://coe.pycfn.com

[R59] 发 POST JSON
来源：http://szf.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kra.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://mmk.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mtk.pengpengdd.cyou

[R61] 磁盘占用
来源：http://tim.zdbjq.cn

df -h;  du -sh *
来源：http://det.hnqzz.top

[R62] 找最占空间的文件
来源：http://pur.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://fvi.sxryk.cn

[R63] 内存与进程
来源：http://xrh.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://xxy.hesvh.cn

[R64] 结束进程
来源：http://dog.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://ubc.jiagoushi.top

[R65] 查看端口占用
来源：http://exq.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://euc.smart0.xyz

[R66] 定时任务
来源：http://jjq.kuanghao11.cn

crontab -e;  crontab -l
来源：http://efe.sysykeji.top

[R67] 生成随机十六进制串
来源：http://jwz.andypj.xyz

openssl rand -hex 16
来源：http://sfk.yueranfly.top

[R68] 计算文件校验值
来源：http://hfk.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://anc.jinyuanbaomall.cn

[R69] 生成随机密码
来源：http://hrh.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://bpg.ydzc1.top

[R70] 时间戳与互转
来源：http://xmd.svipenyu.cn

date +%s;  date -d @1700000000
来源：http://ycb.yueranfly.top

[R71] 日期格式化
来源：http://iuw.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://gcr.cucudq.cn

[R72] 等待端口就绪
来源：http://tmj.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rcm.ctjpmb.com

[R73] 分割大日志
来源：http://gkw.yongpay.top

split -l 1000 big.log part_
来源：http://pen.dashuyun.cn

[R74] 批量重命名
来源：http://rdr.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vos.ehwqpu.com

[R75] 导出环境变量
来源：http://cbq.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://yyd.yuanzhike.top

[R76] 使用临时文件
来源：http://khf.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xii.yvedp.cn

[R77] 读取用户输入
来源：http://wsj.yangfankeji.com

read -rp "请输入: " ans
来源：http://gci.jqgfzy.top

[R78] 交互式菜单
来源：http://hex.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tau.xziqi.cn

[R79] 解析命令行选项
来源：http://rqq.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mtc.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://bpq.gogol.net.cn

time ./run.sh
来源：http://kic.xinyue.icu

================================================================================
来源：http://cow.tian-w.cn

S. C / C++ 专题
来源：http://qam.jianghu66.top

================================================================================
来源：http://reo.epnwcf.com

[S01] C：Hello World
来源：http://mtg.meibo888.top

#include <stdio.h>
来源：http://zoy.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pqn.gzhubu.top

[S02] C：变量与格式化输出
来源：http://koz.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://lug.sysykeji.top

[S03] C：读入整数
来源：http://nlr.iojbl.cn

int x; scanf("%d", &x);
来源：http://kvz.sufxvd.cn

[S04] C：字符串复制
来源：http://ivq.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://ywt.yueranfly.top

[S05] C：字符串长度
来源：http://qde.yanxiufei.cn

strlen(s)
来源：http://htq.hfpthk.cn

[S06] C：字符串比较
来源：http://sta.yuanzhike.top

strcmp(a, b) == 0
来源：http://exb.xinyue.icu

[S07] C：数组遍历求和
来源：http://ekq.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ziq.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://twz.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kuo.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://cbx.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aff.meibo888.top

[S10] C：指针与解引用
来源：http://iqd.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://ugu.ehwqpu.com

[S11] C：逐行读文件
来源：http://lqp.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://vae.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hep.daria6918.cn

fclose(f);
来源：http://ccv.ywan-chungtsiang.top

[S12] C：写文件
来源：http://drw.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oor.xinyue.icu

[S13] C：宏定义
来源：http://vwk.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gez.yanxiufei.cn

[S14] C：枚举
来源：http://qtl.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://hbz.wangdashe.top

[S15] C：类型转换
来源：http://wft.jyoumei.cn

(double) a / b
来源：http://wqa.vqdsnc.cn

[S16] C：位操作置位
来源：http://bid.tanke756.top

x |= (1 << 3);
来源：http://lgq.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://ohl.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lmj.dianchejie.cn

[S18] C：命令行参数
来源：http://zkh.xylfe.cn

int main(int argc, char **argv)
来源：http://frp.zdbjq.cn

[S19] C：快速排序
来源：http://aud.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://giy.uphjek.com

[S20] C：二分查找
来源：http://wss.ydzc1.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zyo.yueranfly.top

[S21] C：字符类别判断
来源：http://rdo.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nun.kuanghao11.cn

[S22] C：字符串转数字
来源：http://olx.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zag.ywan-chungtsiang.top

[S23] C：随机数
来源：http://lsv.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kqt.birdmap.top

[S24] C：获取本地时间
来源：http://ngt.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zqc.guowangkeji.top

[S25] C：内存拷贝
来源：http://vwu.shuidangran.top

memcpy(dst, src, n);
来源：http://sxe.haohaochexian.top

[S26] C：内存清零
来源：http://mka.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://qxn.shangyingyoupin.top

[S27] C：定义常量
来源：http://xol.pycfn.com

const double PI = 3.14159;
来源：http://oqw.bbcook.cn

[S28] C：静态变量
来源：http://blq.tianlin.xyz

static int counter = 0;
来源：http://voz.zdbjq.cn

[S29] C：变参函数
来源：http://llq.vqdsnc.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://csc.jinqigufen.top

[S30] C：头文件保护
来源：http://gyc.dianchejie.cn

#ifndef X_H
来源：http://viv.gogol.net.cn

#define X_H
来源：http://ris.jlsjyb.cn

#endif
来源：http://bgd.yongpay.top

[S31] C++：Hello World
来源：http://inx.gaohongyu789.top

#include <iostream>
来源：http://mnf.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://uvi.sysykeji.top

[S32] C++：字符串
来源：http://hxo.jqgfzy.top

std::string s = "hi";  s += "!";
来源：http://jyb.hysaishi.cn

[S33] C++：vector 增删
来源：http://hst.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xai.guannengcc.top

[S34] C++：遍历 vector
来源：http://iye.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://cpq.wangshuangyany.cn

[S35] C++：map
来源：http://xam.yueranfly.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pdy.zhongyouzk.top

[S36] C++：unordered_map
来源：http://dse.sweek.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fiq.dianchejie.cn

[S37] C++：set
来源：http://jsg.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wso.zdbjq.cn

[S38] C++：排序
来源：http://vjn.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://slx.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://ifk.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nuy.snrcjt.cn

[S40] C++：查找元素
来源：http://jfs.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kdn.jinqigufen.top

[S41] C++：类与构造函数
来源：http://jib.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://luv.pycfn.com

[S42] C++：继承与虚函数
来源：http://tpm.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://che.zhijiandao.cn

[S43] C++：智能指针
来源：http://nlu.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://fuk.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://tzr.zhijiandao.cn

void inc(int &x) { ++x; }
来源：http://mmo.hfpthk.cn

[S45] C++：lambda
来源：http://hmw.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://ads.ybcxt.top

[S46] C++：函数模板
来源：http://fua.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hwu.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://swk.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pub.yonumen.top

[S48] C++：逐行读文件
来源：http://xvl.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mdz.fanxiaobao.xyz


<!-- 参考信息 -->