代发 wailian999

[Q80] 字符串截取
来源：http://upj.zhiwuduotai.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aky.ehwqpu.com

[Q81] 字符串替换
来源：http://sxn.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hfq.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://scq.yuanzhike.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wor.yj20258888.top

[Q83] 大小写转换
来源：http://rpr.zhongyouzk.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lvz.cheryme.top

[Q84] 去除首尾空格
来源：http://wsg.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://qam.tianlin.xyz

[Q85] 数值取整
来源：http://qmn.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nxl.xuetiantiany.cn

[Q86] 读取 JSON 字段
来源：http://ksu.jinghuilouyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yxm.hcnkem.com

[Q87] JSON 字段做条件
来源：http://hpj.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zlt.fengsongda.top

[Q88] 行转列（条件聚合）
来源：http://ddv.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wzj.birdmap.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xpz.andypj.xyz

[Q89] 判断表是否存在
来源：http://sce.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eji.zhoulong.xyz

[Q90] 生成序号列
来源：http://hgy.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rcq.ybcxt.top

================================================================================
来源：http://jwq.sufxvd.cn

R. Bash 专题
来源：http://bii.ehwqpu.com

================================================================================
来源：http://yif.zhaomingkeji.xyz

[R01] shebang 与严格模式
来源：http://nsa.shuidangran.top

#!/usr/bin/env bash
来源：http://hrh.nwbrower.top

set -euo pipefail
来源：http://lla.guowangkeji.top

[R02] 变量赋值与使用
来源：http://vka.cheryme.top

name="Tom"; echo "$name"
来源：http://ird.shzxlz.cn

[R03] 只读变量
来源：http://nmg.guowangkeji.top

readonly PI=3.14
来源：http://kko.zhixingplan.top

[R04] 位置参数
来源：http://sey.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fwx.daxiang520.top

[R05] 参数默认值
来源：http://sne.jinyuanbaomall.cn

name="${1:-default}"
来源：http://wlr.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://ntf.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hin.zhixingplan.top

[R07] if 判断文件
来源：http://zqk.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nck.pengpengdd.cyou

[R08] 数值比较
来源：http://oxl.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dtk.yuxming.cn

[R09] 字符串比较
来源：http://lld.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mrn.jinqigfzy.top

[R10] 正则匹配
来源：http://qqr.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ntx.sysykeji.top

[R11] case 多分支
来源：http://fjs.pengpengdd.cyou

case "$1" in
来源：http://coc.iojbl.cn

start) echo "启动" ;;
来源：http://byl.hysaishi.cn

stop)  echo "停止" ;;
来源：http://qmd.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://ytt.pycfn.com

esac
来源：http://lxf.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://xju.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://urw.vehdjk.com

[R13] for 计数循环
来源：http://xnp.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://riu.hammf.cn

[R14] C 风格 for
来源：http://knt.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://axc.tianlin.xyz

[R15] while 逐行读文件
来源：http://ayo.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mko.jqgufenzy.top

[R16] until 等待条件
来源：http://cei.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yii.gogol.net.cn

[R17] 数组定义与取值
来源：http://nlv.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://kcd.9152youxi.cn

[R18] 遍历数组
来源：http://yfs.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dvu.gogol.net.cn

[R19] 数组长度
来源：http://txo.yj20258888.top

echo "${#arr[@]}"
来源：http://nvl.birdmap.top

[R20] 关联数组（字典）
来源：http://gwi.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hon.yongpay.top

[R21] 字符串长度
来源：http://hxm.snrcjt.cn

echo "${#s}"
来源：http://jwu.nanxuanxn.top

[R22] 截取子串
来源：http://tdg.sweek.top

echo "${s:0:5}"
来源：http://vrt.yfazqb.com

[R23] 字符串替换
来源：http://yaw.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fws.9152youxi.cn

[R24] 大小写转换
来源：http://jyz.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zyc.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://mob.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kmn.zhengqikj.top

[R26] 命令替换
来源：http://wap.xinyue.icu

now=$(date +%F); echo "$now"
来源：http://bwb.xingfuxueyuan.xyz

[R27] 算术展开
来源：http://iry.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://bxm.cucudq.cn

[R28] 浮点运算
来源：http://mpt.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://kdx.snrcjt.cn

[R29] 定义函数
来源：http://ozq.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dor.quarkkingdee.top

[R30] 函数返回状态码
来源：http://gtw.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://pao.guowangkeji.top

[R31] 局部变量
来源：http://apb.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://fzm.iojbl.cn

[R32] 参数个数校验
来源：http://ger.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xkx.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://cra.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xxk.vqdsnc.cn

[R34] 退出时清理
来源：http://pnk.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://mkz.hesvh.cn

[R35] 后台执行并等待
来源：http://xxy.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zap.hesvh.cn

[R36] 并发执行多个任务
来源：http://mhm.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aao.wangdashe.top

[R37] 把输出赋给变量
来源：http://uom.cucudq.cn

files=$(ls -1)
来源：http://uki.shuidangran.top

[R38] 管道串联
来源：http://uny.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://ook.yj20258.top

[R39] 重定向标准输出与错误
来源：http://mob.havefunace.top

cmd > out.log 2>&1
来源：http://xef.epnwcf.com

[R40] 追加写日志
来源：http://pyz.gogol.net.cn

echo "log" >> out.log
来源：http://fwn.yuanzhike.top

[R41] 丢弃输出
来源：http://feo.yongpay.top

cmd >/dev/null 2>&1
来源：http://xtu.fzhhl.top

[R42] 输入重定向
来源：http://qqy.andypj.xyz

wc -l < a.txt
来源：http://xbj.cashguo.top

[R43] 按名字查找文件
来源：http://cls.dashuyun.cn

find . -name "*.log" -type f
来源：http://vvv.c1oappe.top

[R44] 按修改时间查找
来源：http://pgi.aizwys.cn

find . -mtime -7 -type f
来源：http://kji.sjlbkw.cn

[R45] 批量删除
来源：http://zee.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://ybv.cheryme.top

[R46] 递归替换文件内容
来源：http://rgn.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iqr.jianghu66.top

[R47] sed 单行替换
来源：http://exu.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ehj.bbcook.cn

[R48] awk 取指定列
来源：http://dsd.zhengqikj.top

awk '{print $1, $3}' a.txt
来源：http://nga.cucudq.cn

[R49] awk 带条件
来源：http://rcv.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://krc.tian-w.cn

[R50] awk 求和
来源：http://hdw.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rqr.cucudq.cn

[R51] 排序去重取前几
来源：http://lhe.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nxd.sysykeji.top

[R52] 统计行数
来源：http://oqf.hammf.cn

wc -l a.txt
来源：http://lzk.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://qxx.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vit.hywenlv.cn

[R54] 比较两个文件
来源：http://bti.epnwcf.com

diff a.txt b.txt
来源：http://uvq.smart0.xyz

[R55] 压缩与解压
来源：http://tgl.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ili.ivvv.top

[R56] 远程拷贝
来源：http://csy.xuetiantiany.cn

scp file user@host:/path/
来源：http://wsl.quarkkingdee.top

[R57] 远程执行命令
来源：http://ves.zhengqikj.top

ssh user@host 'uptime'
来源：http://sqc.jinqigufen.top

[R58] 下载文件
来源：http://jcp.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://acd.xylfe.cn

[R59] 发 POST JSON
来源：http://lob.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xyk.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://hbu.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bfb.pengpengdd.cyou

[R61] 磁盘占用
来源：http://bsp.xuanzx.com

df -h;  du -sh *
来源：http://dxu.hfpthk.cn

[R62] 找最占空间的文件
来源：http://ikx.fktsv.cn

du -ah . | sort -rh | head -10
来源：http://gwm.tian-w.cn

[R63] 内存与进程
来源：http://zhs.316326.xyz

free -h;  ps aux | grep nginx
来源：http://pcz.bbcook.cn

[R64] 结束进程
来源：http://cox.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://wem.fzhhl.top

[R65] 查看端口占用
来源：http://hly.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://olh.hnxiangtu.top

[R66] 定时任务
来源：http://zra.vqdsnc.cn

crontab -e;  crontab -l
来源：http://nrb.iojbl.cn

[R67] 生成随机十六进制串
来源：http://lru.zhixingplan.top

openssl rand -hex 16
来源：http://fmw.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://omx.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://njq.chenjidiqi.icu

[R69] 生成随机密码
来源：http://bxn.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://nyn.hysaishi.cn

[R70] 时间戳与互转
来源：http://vye.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://rts.snrcjt.cn

[R71] 日期格式化
来源：http://zrl.0kj1m.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fas.sysykeji.top

[R72] 等待端口就绪
来源：http://leu.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gjx.chenjidiqi.icu

[R73] 分割大日志
来源：http://zeg.316326.xyz

split -l 1000 big.log part_
来源：http://ggp.52xcode.cn

[R74] 批量重命名
来源：http://beq.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://csm.jqgfzy.top

[R75] 导出环境变量
来源：http://tti.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://wcx.bbcook.cn

[R76] 使用临时文件
来源：http://wwt.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nut.daria6918.cn

[R77] 读取用户输入
来源：http://tvi.cucudq.cn

read -rp "请输入: " ans
来源：http://zyw.vqdsnc.cn

[R78] 交互式菜单
来源：http://agq.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://rmp.cqqwz.cn

[R79] 解析命令行选项
来源：http://enb.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jsz.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://jhr.nanxuanxn.top

time ./run.sh
来源：http://mve.9152youxi.cn

================================================================================
来源：http://opt.cdnleiting.top

S. C / C++ 专题
来源：http://hav.zdqjudy.top

================================================================================
来源：http://zax.hcnkem.com

[S01] C：Hello World
来源：http://ehu.xuetiantiany.cn

#include <stdio.h>
来源：http://irz.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xhv.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://ekm.yanxiufei.cn

int a = 10; printf("%d\n", a);
来源：http://ajo.zhijiandao.cn

[S03] C：读入整数
来源：http://ltj.316326.xyz

int x; scanf("%d", &x);
来源：http://oep.jinqigufen.top

[S04] C：字符串复制
来源：http://lpr.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kag.yanxiufei.cn

[S05] C：字符串长度
来源：http://gta.nanxinkj.top

strlen(s)
来源：http://zye.sjlbkw.cn

[S06] C：字符串比较
来源：http://xad.fzhhl.top

strcmp(a, b) == 0
来源：http://mqh.316326.xyz

[S07] C：数组遍历求和
来源：http://lwu.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iyx.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://wio.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rys.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://krs.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jqa.yanxiufei.cn

[S10] C：指针与解引用
来源：http://izx.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://mfr.hywenlv.cn

[S11] C：逐行读文件
来源：http://mpo.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://rmk.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://anj.meibo888.top

fclose(f);
来源：http://abq.hfpthk.cn

[S12] C：写文件
来源：http://uxk.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zpa.316326.xyz

[S13] C：宏定义
来源：http://kmy.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jag.ctjpmb.com

[S14] C：枚举
来源：http://shr.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://ifd.xinyue.icu

[S15] C：类型转换
来源：http://dkd.52xcode.cn

(double) a / b
来源：http://lgc.hysaishi.cn

[S16] C：位操作置位
来源：http://yja.andypj.xyz

x |= (1 << 3);
来源：http://zgn.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://sht.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ona.yuanzhike.top

[S18] C：命令行参数
来源：http://aay.guannengcc.top

int main(int argc, char **argv)
来源：http://ziu.yongpay.top

[S19] C：快速排序
来源：http://eow.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://adp.nanxuanxn.top

[S20] C：二分查找
来源：http://ubu.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zzq.zycfv.cn

[S21] C：字符类别判断
来源：http://qyj.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cah.meibo888.top

[S22] C：字符串转数字
来源：http://qvl.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://xnj.jianghu66.top

[S23] C：随机数
来源：http://qyr.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qsq.hesvh.cn

[S24] C：获取本地时间
来源：http://obv.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cte.cdnleiting.top

[S25] C：内存拷贝
来源：http://hoy.gzhubu.top

memcpy(dst, src, n);
来源：http://imy.xylfe.cn

[S26] C：内存清零
来源：http://xve.birdmap.top

memset(a, 0, sizeof a);
来源：http://fmg.cashguo.top

[S27] C：定义常量
来源：http://bmb.0kj1m.cn

const double PI = 3.14159;
来源：http://vsi.shanyushiyangtech.top

[S28] C：静态变量
来源：http://bkw.guannengcc.top

static int counter = 0;
来源：http://bhm.jinghuilouyu.cn

[S29] C：变参函数
来源：http://eei.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pcy.cqqwz.cn

[S30] C：头文件保护
来源：http://dly.zhixingplan.top

#ifndef X_H
来源：http://vzp.cashguo.top

#define X_H
来源：http://jin.cheryme.top

#endif
来源：http://bjo.xziqi.cn

[S31] C++：Hello World
来源：http://zyv.zhoulong.xyz

#include <iostream>
来源：http://ezi.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://wia.aibaodan.cn

[S32] C++：字符串
来源：http://uxk.ydjk.org.cn

std::string s = "hi";  s += "!";
来源：http://mtw.zhixingplan.top

[S33] C++：vector 增删
来源：http://hdp.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hoz.jianghu66.top

[S34] C++：遍历 vector
来源：http://okm.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://huu.tianlin.xyz

[S35] C++：map
来源：http://koq.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kyx.zdbjq.cn

[S36] C++：unordered_map
来源：http://jee.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xao.yueranfly.top

[S37] C++：set
来源：http://qox.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gft.hysaishi.cn

[S38] C++：排序
来源：http://qyr.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://pui.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://gjz.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ywu.zhengqikj.top

[S40] C++：查找元素
来源：http://eji.cucudq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uvu.0kj1m.cn

[S41] C++：类与构造函数
来源：http://fot.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aho.zycfv.cn

[S42] C++：继承与虚函数
来源：http://uei.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://xee.yvedp.cn

[S43] C++：智能指针
来源：http://ely.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://wik.zdqjudy.top

[S44] C++：引用传参
来源：http://ykn.yfazqb.com

void inc(int &x) { ++x; }
来源：http://vbv.dianchejie.cn

[S45] C++：lambda
来源：http://gqy.shzxlz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ald.chenlongwang.top

[S46] C++：函数模板
来源：http://ald.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wst.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://zan.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lvg.shzxlz.cn

[S48] C++：逐行读文件
来源：http://viz.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://bor.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://hsx.hnxiangtu.top

[S49] C++：写文件
来源：http://mqy.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eny.zdqjudy.top

[S50] C++：格式化数字
来源：http://ncy.zhijiandao.cn


<!-- 参考信息 -->