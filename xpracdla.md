代发 wailian999

[Q78] 当前时间
来源：http://cvb.pycfn.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hwc.jianghu66.top

[Q79] 字符串拼接
来源：http://dbm.yuanzhike.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sxk.jlsjyb.cn

[Q80] 字符串截取
来源：http://hrw.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://htr.hysaishi.cn

[Q81] 字符串替换
来源：http://bdw.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ukz.svipenyu.cn

[Q82] 字符长度与字节长度
来源：http://ejg.cucudq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rln.svipenyu.cn

[Q83] 大小写转换
来源：http://roz.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://spn.aibaodan.cn

[Q84] 去除首尾空格
来源：http://jrs.tanke756.top

SELECT TRIM(name) FROM users;
来源：http://iil.jlsjyb.cn

[Q85] 数值取整
来源：http://jno.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://snb.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://zir.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tqj.cashguo.top

[Q87] JSON 字段做条件
来源：http://vmv.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mro.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://jdi.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lct.ivvv.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jeb.redwolf501.top

[Q89] 判断表是否存在
来源：http://zsv.daxiang520.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://snf.xinyue.icu

[Q90] 生成序号列
来源：http://ogd.yangfankeji.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nsb.zycfv.cn

================================================================================
来源：http://xhm.hnqzz.top

R. Bash 专题
来源：http://ewc.havefunace.top

================================================================================
来源：http://dht.cucudq.cn

[R01] shebang 与严格模式
来源：http://oah.havefunace.top

#!/usr/bin/env bash
来源：http://rdv.dianchejie.cn

set -euo pipefail
来源：http://axy.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://vel.yangfankeji.com

name="Tom"; echo "$name"
来源：http://lda.yj202588.top

[R03] 只读变量
来源：http://ydb.sxryk.cn

readonly PI=3.14
来源：http://jje.tianlin.xyz

[R04] 位置参数
来源：http://ama.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sdf.feifeiyinyue.top

[R05] 参数默认值
来源：http://gnp.chenzaomai.com

name="${1:-default}"
来源：http://itc.yangfankeji.com

[R06] 判断命令是否存在
来源：http://ipb.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gzw.jqgufenzy.top

[R07] if 判断文件
来源：http://qrj.birdmap.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lhz.tarul.cn

[R08] 数值比较
来源：http://hyk.gotoacloud.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sqt.gotoacloud.top

[R09] 字符串比较
来源：http://jiw.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dat.bjfxy.top

[R10] 正则匹配
来源：http://exc.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://awn.ehwqpu.com

[R11] case 多分支
来源：http://rme.hfpthk.cn

case "$1" in
来源：http://zfz.yj202588.top

start) echo "启动" ;;
来源：http://cll.shuidangran.top

stop)  echo "停止" ;;
来源：http://ywn.jinghuilouyu.cn

*)     echo "未知命令" ;;
来源：http://nlf.jinghuilouyu.cn

esac
来源：http://ywq.gotoacloud.top

[R12] for 遍历文件
来源：http://xrf.gogol.net.cn

for f in *.txt; do echo "$f"; done
来源：http://lda.svipenyu.cn

[R13] for 计数循环
来源：http://lki.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://lqz.shangyingyoupin.top

[R14] C 风格 for
来源：http://uav.meibo888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kns.hnqzz.top

[R15] while 逐行读文件
来源：http://wzn.mhx1999.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ajf.gaohongyu789.top

[R16] until 等待条件
来源：http://pih.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gge.xuanzx.com

[R17] 数组定义与取值
来源：http://rds.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://iwd.dianchejie.cn

[R18] 遍历数组
来源：http://xyy.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ilu.sweek.top

[R19] 数组长度
来源：http://efz.sweek.top

echo "${#arr[@]}"
来源：http://oid.zdqjudy.top

[R20] 关联数组（字典）
来源：http://dwy.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://akg.ywan-chungtsiang.top

[R21] 字符串长度
来源：http://auw.haohaochexian.top

echo "${#s}"
来源：http://teg.tian-w.cn

[R22] 截取子串
来源：http://ecv.cdnleiting.top

echo "${s:0:5}"
来源：http://vls.52xcode.cn

[R23] 字符串替换
来源：http://osl.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hdo.cheryme.top

[R24] 大小写转换
来源：http://fnu.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://jwt.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://hdz.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fzo.nwbrower.top

[R26] 命令替换
来源：http://jqz.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://pqy.cucudq.cn

[R27] 算术展开
来源：http://yly.yangfankeji.com

echo $((1 + 2 * 3))
来源：http://toq.sweek.top

[R28] 浮点运算
来源：http://ets.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://iei.hesvh.cn

[R29] 定义函数
来源：http://igp.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://twv.haohaochexian.top

[R30] 函数返回状态码
来源：http://rgi.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://exg.zhixingplan.top

[R31] 局部变量
来源：http://ugs.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://bok.yj20258888.top

[R32] 参数个数校验
来源：http://xlp.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pii.guowangkeji.top

[R33] 捕获错误并提示行号
来源：http://bhk.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gwd.xziqi.cn

[R34] 退出时清理
来源：http://toe.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://agq.cashguo.top

[R35] 后台执行并等待
来源：http://jeh.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xjd.feifeiyinyue.top

[R36] 并发执行多个任务
来源：http://lfc.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gip.zhixingplan.top

[R37] 把输出赋给变量
来源：http://art.dianchejie.cn

files=$(ls -1)
来源：http://jkf.pengpengdd.cyou

[R38] 管道串联
来源：http://nbw.tarul.cn

cat a.txt | grep -i error | wc -l
来源：http://cac.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://rtb.zhoulong.xyz

cmd > out.log 2>&1
来源：http://kvl.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://hrp.zhiwuduotai.top

echo "log" >> out.log
来源：http://xzw.hnxiangtu.top

[R41] 丢弃输出
来源：http://eua.tian-w.cn

cmd >/dev/null 2>&1
来源：http://srs.fzhhl.top

[R42] 输入重定向
来源：http://zio.snrcjt.cn

wc -l < a.txt
来源：http://zal.fzhhl.top

[R43] 按名字查找文件
来源：http://lon.gotoacloud.top

find . -name "*.log" -type f
来源：http://pmc.xinyue.icu

[R44] 按修改时间查找
来源：http://put.redwolf501.top

find . -mtime -7 -type f
来源：http://azq.yongpay.top

[R45] 批量删除
来源：http://nbr.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://npj.aizwys.cn

[R46] 递归替换文件内容
来源：http://epo.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wsh.52xcode.cn

[R47] sed 单行替换
来源：http://zgb.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sel.chenjidiqi.icu

[R48] awk 取指定列
来源：http://hjn.52xcode.cn

awk '{print $1, $3}' a.txt
来源：http://drc.yj20258888.top

[R49] awk 带条件
来源：http://tdd.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rqa.birdmap.top

[R50] awk 求和
来源：http://vyr.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://yhj.yfazqb.com

[R51] 排序去重取前几
来源：http://zed.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://pxk.xuanzx.com

[R52] 统计行数
来源：http://jpp.sxryk.cn

wc -l a.txt
来源：http://bty.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://abl.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://udm.cqqwz.cn

[R54] 比较两个文件
来源：http://znq.zhengqikj.top

diff a.txt b.txt
来源：http://tjn.hysaishi.cn

[R55] 压缩与解压
来源：http://iyw.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bxv.jianghu66.top

[R56] 远程拷贝
来源：http://dgn.mhx1999.top

scp file user@host:/path/
来源：http://ydo.yfazqb.com

[R57] 远程执行命令
来源：http://xkz.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://qaz.pycfn.com

[R58] 下载文件
来源：http://ove.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qco.bjfxy.top

[R59] 发 POST JSON
来源：http://erd.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fup.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://gzv.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bjl.hywenlv.cn

[R61] 磁盘占用
来源：http://osy.ppjwa.cn

df -h;  du -sh *
来源：http://jnz.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://kan.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://smg.hongshengwenyu.top

[R63] 内存与进程
来源：http://orv.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://ktt.c1oappe.top

[R64] 结束进程
来源：http://iql.jianghu66.top

kill -9 $(pgrep -f app.py)
来源：http://tmt.fengsongda.top

[R65] 查看端口占用
来源：http://qqf.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lqp.ehwqpu.com

[R66] 定时任务
来源：http://jof.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://jkr.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://jin.jyoumei.cn

openssl rand -hex 16
来源：http://kqh.pycfn.com

[R68] 计算文件校验值
来源：http://yon.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://rae.hnqzz.top

[R69] 生成随机密码
来源：http://yco.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://laa.chenlongwang.top

[R70] 时间戳与互转
来源：http://fkh.xylfe.cn

date +%s;  date -d @1700000000
来源：http://ver.chenjidiqi.icu

[R71] 日期格式化
来源：http://gys.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jyc.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://zjt.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hxd.yuanzhike.top

[R73] 分割大日志
来源：http://zqp.zhengqikj.top

split -l 1000 big.log part_
来源：http://thq.fengsongda.top

[R74] 批量重命名
来源：http://avs.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jlg.hongshengwenyu.top

[R75] 导出环境变量
来源：http://yyx.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://vak.bbcook.cn

[R76] 使用临时文件
来源：http://dmf.xylfe.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nib.yueranfly.top

[R77] 读取用户输入
来源：http://jzt.smart0.xyz

read -rp "请输入: " ans
来源：http://ftx.dianchejie.cn

[R78] 交互式菜单
来源：http://zjm.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://may.daxiang520.top

[R79] 解析命令行选项
来源：http://zkh.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ubl.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://aev.jyoumei.cn

time ./run.sh
来源：http://lhx.zdqjudy.top

================================================================================
来源：http://agb.nanxinkj.top

S. C / C++ 专题
来源：http://yco.hywenlv.cn

================================================================================
来源：http://rnz.shanyushiyangtech.top

[S01] C：Hello World
来源：http://tgg.havefunace.top

#include <stdio.h>
来源：http://cma.pengpengdd.cyou

int main(void) { printf("Hello\n"); return 0; }
来源：http://xri.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://wcf.ctjpmb.com

int a = 10; printf("%d\n", a);
来源：http://sba.yuanzhike.top

[S03] C：读入整数
来源：http://cuv.xinyue.icu

int x; scanf("%d", &x);
来源：http://dng.hysaishi.cn

[S04] C：字符串复制
来源：http://wrq.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://ape.jinqigfzy.top

[S05] C：字符串长度
来源：http://lmc.fengsongda.top

strlen(s)
来源：http://wci.yonumen.top

[S06] C：字符串比较
来源：http://mbf.zycfv.cn

strcmp(a, b) == 0
来源：http://mto.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://vjo.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vdw.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://wew.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yxn.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://mhd.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jae.yuxming.cn

[S10] C：指针与解引用
来源：http://vhd.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://rfx.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://cxr.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://wgs.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://soc.iojbl.cn

fclose(f);
来源：http://dzp.tianlin.xyz

[S12] C：写文件
来源：http://hga.guannengcc.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jep.cdnleiting.top

[S13] C：宏定义
来源：http://ekz.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iee.zhoulong.xyz

[S14] C：枚举
来源：http://aov.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://xho.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://skg.guannengcc.top

(double) a / b
来源：http://zos.nanxinkj.top

[S16] C：位操作置位
来源：http://mas.zhiwuduotai.top

x |= (1 << 3);
来源：http://mqb.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://btx.jianghu66.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yaf.epnwcf.com

[S18] C：命令行参数
来源：http://wno.daria6918.cn

int main(int argc, char **argv)
来源：http://fgu.wangdashe.top

[S19] C：快速排序
来源：http://mon.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://afr.jyoumei.cn

[S20] C：二分查找
来源：http://fza.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tct.316326.xyz

[S21] C：字符类别判断
来源：http://hjv.yvedp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gow.xylfe.cn

[S22] C：字符串转数字
来源：http://wqe.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://jeb.zhiwuduotai.top

[S23] C：随机数
来源：http://hdi.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ghc.dashuyun.cn

[S24] C：获取本地时间
来源：http://ohy.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gif.yj20258888.top

[S25] C：内存拷贝
来源：http://tbc.fengsongda.top

memcpy(dst, src, n);
来源：http://ocz.xuetiantiany.cn

[S26] C：内存清零
来源：http://ttz.fzhhl.top

memset(a, 0, sizeof a);
来源：http://wau.xinyue.icu

[S27] C：定义常量
来源：http://woa.tanke756.top

const double PI = 3.14159;
来源：http://tmz.chenzaomai.com

[S28] C：静态变量
来源：http://bod.xuetiantiany.cn

static int counter = 0;
来源：http://uvv.cdnleiting.top

[S29] C：变参函数
来源：http://byk.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pwx.ctjpmb.com

[S30] C：头文件保护
来源：http://fhv.fanxiaobao.xyz

#ifndef X_H
来源：http://dgf.jinqigfzy.top

#define X_H
来源：http://euo.pycfn.com

#endif
来源：http://qgj.bjfxy.top

[S31] C++：Hello World
来源：http://fty.svipenyu.cn

#include <iostream>
来源：http://koc.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://olv.gotoacloud.top

[S32] C++：字符串
来源：http://eup.yj20258888.top

std::string s = "hi";  s += "!";
来源：http://duy.jinghuilouyu.cn

[S33] C++：vector 增删
来源：http://agk.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mkt.yj20258.top

[S34] C++：遍历 vector
来源：http://kyx.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://ayf.sxryk.cn

[S35] C++：map
来源：http://cph.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vgb.ppjwa.cn

[S36] C++：unordered_map
来源：http://pmr.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gtv.yj20258.top

[S37] C++：set
来源：http://chr.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sdu.birdmap.top

[S38] C++：排序
来源：http://xjw.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://shx.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://mit.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mhb.tian-w.cn

[S40] C++：查找元素
来源：http://vbr.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xgz.haohaochexian.top

[S41] C++：类与构造函数
来源：http://rum.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://irr.nwbrower.top

[S42] C++：继承与虚函数
来源：http://pyq.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://hnd.sweek.top

[S43] C++：智能指针
来源：http://fsi.yanxiufei.cn

auto p = std::make_unique<int>(5);
来源：http://pka.daria6918.cn

[S44] C++：引用传参
来源：http://hbb.aizwys.cn

void inc(int &x) { ++x; }
来源：http://ptt.vqdsnc.cn

[S45] C++：lambda
来源：http://rvu.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vhq.feifeiyinyue.top

[S46] C++：函数模板
来源：http://vhg.pycfn.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nso.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://hcf.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yzf.vehdjk.com

[S48] C++：逐行读文件
来源：http://enz.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://ynw.shanyushiyangtech.top


<!-- 参考信息 -->