代发 wailian999

[Q82] 字符长度与字节长度
来源：http://wvz.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://knr.yangfankeji.com

[Q83] 大小写转换
来源：http://tot.vqdsnc.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bfm.dashuyun.cn

[Q84] 去除首尾空格
来源：http://vkw.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://irq.feifeiyinyue.top

[Q85] 数值取整
来源：http://gjd.xingfuxueyuan.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cor.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://vea.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cet.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://tuo.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lpx.hcnkem.com

[Q88] 行转列（条件聚合）
来源：http://tib.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ocy.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://brh.chenjidiqi.icu

[Q89] 判断表是否存在
来源：http://mcl.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fhg.zdqjudy.top

[Q90] 生成序号列
来源：http://fue.kuanghao11.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xkp.aizwys.cn

================================================================================
来源：http://bdm.snrcjt.cn

R. Bash 专题
来源：http://qrn.yueranfly.top

================================================================================
来源：http://fio.ivvv.top

[R01] shebang 与严格模式
来源：http://vec.tianlin.xyz

#!/usr/bin/env bash
来源：http://gby.hysaishi.cn

set -euo pipefail
来源：http://kaq.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://rwh.xziqi.cn

name="Tom"; echo "$name"
来源：http://cuj.gaohongyu789.top

[R03] 只读变量
来源：http://lqg.ehwqpu.com

readonly PI=3.14
来源：http://iaf.ydzc1.top

[R04] 位置参数
来源：http://jzj.ybcxt.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dnl.dianchejie.cn

[R05] 参数默认值
来源：http://ict.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://tbo.aibaodan.cn

[R06] 判断命令是否存在
来源：http://bnl.cashguo.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://unb.yueranfly.top

[R07] if 判断文件
来源：http://egp.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dqx.svipenyu.cn

[R08] 数值比较
来源：http://fkz.zhaomingkeji.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://vsb.ppjwa.cn

[R09] 字符串比较
来源：http://qan.xuetiantiany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yad.fehbvm.com

[R10] 正则匹配
来源：http://spd.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lbl.cucudq.cn

[R11] case 多分支
来源：http://nqp.vqdsnc.cn

case "$1" in
来源：http://epr.pycfn.com

start) echo "启动" ;;
来源：http://fks.sweek.top

stop)  echo "停止" ;;
来源：http://fbs.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://mom.haohaochexian.top

esac
来源：http://nhx.zhijiandao.cn

[R12] for 遍历文件
来源：http://hes.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://czg.tianlin.xyz

[R13] for 计数循环
来源：http://asc.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://vhz.nanxinkj.top

[R14] C 风格 for
来源：http://xvg.nanxuanxn.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hpj.c1oappe.top

[R15] while 逐行读文件
来源：http://ufd.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iqy.yangfankeji.com

[R16] until 等待条件
来源：http://qed.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ckt.gzhubu.top

[R17] 数组定义与取值
来源：http://esw.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://acm.zdbjq.cn

[R18] 遍历数组
来源：http://wrt.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qto.zhaomingkeji.xyz

[R19] 数组长度
来源：http://viw.haohaochexian.top

echo "${#arr[@]}"
来源：http://kre.shanyushiyangtech.top

[R20] 关联数组（字典）
来源：http://vfg.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wpp.hongshengwenyu.top

[R21] 字符串长度
来源：http://ycq.shanyushiyangkeji.top

echo "${#s}"
来源：http://upk.hfpthk.cn

[R22] 截取子串
来源：http://zbi.pycfn.com

echo "${s:0:5}"
来源：http://oex.sysykeji.top

[R23] 字符串替换
来源：http://bog.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fkf.sweek.top

[R24] 大小写转换
来源：http://cdq.gaohongyu789.top

echo "${s^^}"; echo "${s,,}"
来源：http://psb.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://waq.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ekc.c1oappe.top

[R26] 命令替换
来源：http://teg.sweek.top

now=$(date +%F); echo "$now"
来源：http://say.chenlongwang.top

[R27] 算术展开
来源：http://wae.bjfxy.top

echo $((1 + 2 * 3))
来源：http://pqc.pengpengdd.cyou

[R28] 浮点运算
来源：http://pgu.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://wla.yfazqb.com

[R29] 定义函数
来源：http://tin.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://agr.sxryk.cn

[R30] 函数返回状态码
来源：http://kjz.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://ieb.wangshuangyany.cn

[R31] 局部变量
来源：http://sjt.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://xda.smart0.xyz

[R32] 参数个数校验
来源：http://ihb.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lvq.havefunace.top

[R33] 捕获错误并提示行号
来源：http://fvn.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gsi.yj202588.top

[R34] 退出时清理
来源：http://brf.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://glv.svipenyu.cn

[R35] 后台执行并等待
来源：http://nle.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://owi.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://kke.9152youxi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jkr.yangfankeji.com

[R37] 把输出赋给变量
来源：http://bon.hysaishi.cn

files=$(ls -1)
来源：http://ybk.cqqwz.cn

[R38] 管道串联
来源：http://teq.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://thj.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://nmz.sufxvd.cn

cmd > out.log 2>&1
来源：http://brr.52xcode.cn

[R40] 追加写日志
来源：http://yfq.cashguo.top

echo "log" >> out.log
来源：http://qff.bbcook.cn

[R41] 丢弃输出
来源：http://qai.uphjek.com

cmd >/dev/null 2>&1
来源：http://bvl.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://wfs.chenlongwang.top

wc -l < a.txt
来源：http://reb.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://vhf.chenlongwang.top

find . -name "*.log" -type f
来源：http://zjj.tianlin.xyz

[R44] 按修改时间查找
来源：http://epp.jqgfzy.top

find . -mtime -7 -type f
来源：http://lmc.yj20258.top

[R45] 批量删除
来源：http://fyb.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://fka.dianchejie.cn

[R46] 递归替换文件内容
来源：http://ydy.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mvb.yuanzhike.top

[R47] sed 单行替换
来源：http://lgp.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://occ.vehdjk.com

[R48] awk 取指定列
来源：http://uqo.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://lkg.guannengcc.top

[R49] awk 带条件
来源：http://zbh.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://drv.fehbvm.com

[R50] awk 求和
来源：http://rfe.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://pzn.sxryk.cn

[R51] 排序去重取前几
来源：http://wqf.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eri.zhijiandao.cn

[R52] 统计行数
来源：http://iqf.havefunace.top

wc -l a.txt
来源：http://myp.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://fyp.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mlv.zdqjudy.top

[R54] 比较两个文件
来源：http://esg.pycfn.com

diff a.txt b.txt
来源：http://zpj.cucudq.cn

[R55] 压缩与解压
来源：http://fkv.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yny.jinqigufen.top

[R56] 远程拷贝
来源：http://tbn.tian-w.cn

scp file user@host:/path/
来源：http://cdj.epnwcf.com

[R57] 远程执行命令
来源：http://aor.c1oappe.top

ssh user@host 'uptime'
来源：http://jec.tian-w.cn

[R58] 下载文件
来源：http://nsc.zhoulong.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://big.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://fct.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://slg.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://qye.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vhe.chenzaomai.com

[R61] 磁盘占用
来源：http://sug.shangyingyoupin.top

df -h;  du -sh *
来源：http://kss.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://vnq.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://hvr.fanxiaobao.xyz

[R63] 内存与进程
来源：http://qxx.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://ljf.cheryme.top

[R64] 结束进程
来源：http://rod.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://nnt.zhixingplan.top

[R65] 查看端口占用
来源：http://vru.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cto.wangdashe.top

[R66] 定时任务
来源：http://gme.kuanghao11.cn

crontab -e;  crontab -l
来源：http://vhj.bjfxy.top

[R67] 生成随机十六进制串
来源：http://vjk.chenlongwang.top

openssl rand -hex 16
来源：http://knf.hywenlv.cn

[R68] 计算文件校验值
来源：http://hba.guowangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://dzq.yuanzhike.top

[R69] 生成随机密码
来源：http://siz.gotoacloud.top

head -c 16 /dev/urandom | base64
来源：http://gib.xziqi.cn

[R70] 时间戳与互转
来源：http://ult.ivvv.top

date +%s;  date -d @1700000000
来源：http://idp.jyoumei.cn

[R71] 日期格式化
来源：http://chd.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://axn.gogol.net.cn

[R72] 等待端口就绪
来源：http://oln.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gui.pengpengdd.cyou

[R73] 分割大日志
来源：http://czw.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://dms.chenjidiqi.icu

[R74] 批量重命名
来源：http://bcu.jiagoushi.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://khd.nanxinkj.top

[R75] 导出环境变量
来源：http://pvw.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://gwu.aibaodan.cn

[R76] 使用临时文件
来源：http://lcb.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://day.fehbvm.com

[R77] 读取用户输入
来源：http://emh.pycfn.com

read -rp "请输入: " ans
来源：http://qor.daria6918.cn

[R78] 交互式菜单
来源：http://gvn.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ghb.ybcxt.top

[R79] 解析命令行选项
来源：http://txt.fehbvm.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aoc.hfpthk.cn

[R80] 查看脚本执行耗时
来源：http://rkr.birdmap.top

time ./run.sh
来源：http://tcg.wangdashe.top

================================================================================
来源：http://daj.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://toc.yangfankeji.com

================================================================================
来源：http://ltj.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://rvb.hnqzz.top

#include <stdio.h>
来源：http://col.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://isl.birdmap.top

[S02] C：变量与格式化输出
来源：http://jeo.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://uiw.kuanghao11.cn

[S03] C：读入整数
来源：http://cri.snrcjt.cn

int x; scanf("%d", &x);
来源：http://ixd.hfpthk.cn

[S04] C：字符串复制
来源：http://wxj.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://gin.quarkkingdee.top

[S05] C：字符串长度
来源：http://jxt.hammf.cn

strlen(s)
来源：http://qua.shuidangran.top

[S06] C：字符串比较
来源：http://klh.jinqigufen.top

strcmp(a, b) == 0
来源：http://gfi.snrcjt.cn

[S07] C：数组遍历求和
来源：http://cdd.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fua.meibo888.top

[S08] C：动态内存分配与释放
来源：http://dlc.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cqk.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://zfx.yj202588.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nys.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://gqr.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://lei.gaohongyu789.top

[S11] C：逐行读文件
来源：http://whc.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://gae.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nkc.vehdjk.com

fclose(f);
来源：http://zkn.quarkkingdee.top

[S12] C：写文件
来源：http://uuw.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hog.vehdjk.com

[S13] C：宏定义
来源：http://jwn.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rwi.xuetiantiany.cn

[S14] C：枚举
来源：http://nuk.yangfankeji.com

enum Color { RED, GREEN, BLUE };
来源：http://tut.yangfankeji.com

[S15] C：类型转换
来源：http://gby.yangfankeji.com

(double) a / b
来源：http://fxl.zhiwuduotai.top

[S16] C：位操作置位
来源：http://euo.jinghuilouyu.cn

x |= (1 << 3);
来源：http://kpo.sysykeji.top

[S17] C：安全拼接字符串
来源：http://gve.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dug.xinyue.icu

[S18] C：命令行参数
来源：http://dtv.yuanzhike.top

int main(int argc, char **argv)
来源：http://ufj.shuidangran.top

[S19] C：快速排序
来源：http://ivh.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://tpc.hnqzz.top

[S20] C：二分查找
来源：http://nou.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xzw.sjlbkw.cn

[S21] C：字符类别判断
来源：http://yic.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rre.dashuyun.cn

[S22] C：字符串转数字
来源：http://cue.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://mca.xuanzx.com

[S23] C：随机数
来源：http://tqk.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dla.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://ezb.jqgufenzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lbn.redwolf501.top

[S25] C：内存拷贝
来源：http://frx.ybcxt.top

memcpy(dst, src, n);
来源：http://iss.jqgufenzy.top

[S26] C：内存清零
来源：http://bno.cucudq.cn

memset(a, 0, sizeof a);
来源：http://zyo.hnxiangtu.top

[S27] C：定义常量
来源：http://fci.chenzaomai.com

const double PI = 3.14159;
来源：http://jbt.0kj1m.cn

[S28] C：静态变量
来源：http://ayg.zdbjq.cn

static int counter = 0;
来源：http://xjy.vehdjk.com

[S29] C：变参函数
来源：http://ugu.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tak.zhongyouzk.top

[S30] C：头文件保护
来源：http://mbx.52xcode.cn

#ifndef X_H
来源：http://plx.smart0.xyz

#define X_H
来源：http://uoo.yuxming.cn

#endif
来源：http://zji.tanke756.top

[S31] C++：Hello World
来源：http://ejv.feifeiyinyue.top

#include <iostream>
来源：http://fjl.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://xgb.xuanzx.com

[S32] C++：字符串
来源：http://tqt.birdmap.top

std::string s = "hi";  s += "!";
来源：http://xdx.xinyue.icu

[S33] C++：vector 增删
来源：http://bmk.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nyh.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://otd.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://sqt.hfpthk.cn

[S35] C++：map
来源：http://tuu.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gde.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://atd.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qjp.jiagoushi.top

[S37] C++：set
来源：http://eas.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nqz.xziqi.cn

[S38] C++：排序
来源：http://ige.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://xvq.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://xcs.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uoo.yuanzhike.top

[S40] C++：查找元素
来源：http://arj.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bpy.cashguo.top

[S41] C++：类与构造函数
来源：http://oso.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://boe.bbcook.cn

[S42] C++：继承与虚函数
来源：http://lti.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://ghh.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://mft.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://bft.hnqzz.top

[S44] C++：引用传参
来源：http://cds.bjfxy.top

void inc(int &x) { ++x; }
来源：http://ljk.zdqjudy.top

[S45] C++：lambda
来源：http://rmh.pengpengdd.cyou

auto add = [](int a, int b) { return a + b; };
来源：http://ami.fehbvm.com

[S46] C++：函数模板
来源：http://wzb.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mgk.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://ywd.sufxvd.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xxv.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://cwo.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://iki.jinghuilouyu.cn

while (std::getline(in, line)) { }
来源：http://wmw.jqgufenzy.top

[S49] C++：写文件
来源：http://kkp.iojbl.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zag.smart0.xyz

[S50] C++：格式化数字
来源：http://wnq.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mvd.gzhubu.top

[S51] C++：显式类型转换
来源：http://fzd.yuanzhike.top

static_cast<double>(a) / b
来源：http://yej.havefunace.top

[S52] C++：const 与 noexcept
来源：http://zio.birdmap.top


<!-- 参考信息 -->