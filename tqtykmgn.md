代发 wailian999

[Q80] 字符串截取
来源：http://hev.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jcf.aizwys.cn

[Q81] 字符串替换
来源：http://bdw.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ogj.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://qrx.nanxinkj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cej.nanxinkj.top

[Q83] 大小写转换
来源：http://vdp.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vok.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://mas.xuetiantiany.cn

SELECT TRIM(name) FROM users;
来源：http://ieu.xziqi.cn

[Q85] 数值取整
来源：http://nwv.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lxj.havefunace.top

[Q86] 读取 JSON 字段
来源：http://crc.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bqk.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://zma.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uvq.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://urc.zhongyouzk.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rqk.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qtg.yangfankeji.com

[Q89] 判断表是否存在
来源：http://mzv.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sdl.mhx1999.top

[Q90] 生成序号列
来源：http://xgh.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kxc.birdmap.top

================================================================================
来源：http://wpj.jianghu66.top

R. Bash 专题
来源：http://fat.snrcjt.cn

================================================================================
来源：http://iqu.iojbl.cn

[R01] shebang 与严格模式
来源：http://equ.yonumen.top

#!/usr/bin/env bash
来源：http://alr.yfazqb.com

set -euo pipefail
来源：http://sku.tanke756.top

[R02] 变量赋值与使用
来源：http://srq.fehbvm.com

name="Tom"; echo "$name"
来源：http://whs.hesvh.cn

[R03] 只读变量
来源：http://fno.zdqjudy.top

readonly PI=3.14
来源：http://lkw.haohaochexian.top

[R04] 位置参数
来源：http://acb.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ped.hfpthk.cn

[R05] 参数默认值
来源：http://dcw.cheryme.top

name="${1:-default}"
来源：http://cdc.tianlin.xyz

[R06] 判断命令是否存在
来源：http://auo.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sua.andypj.xyz

[R07] if 判断文件
来源：http://wqp.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wms.tanke756.top

[R08] 数值比较
来源：http://rye.bbcook.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://njj.svipenyu.cn

[R09] 字符串比较
来源：http://eip.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zxb.xziqi.cn

[R10] 正则匹配
来源：http://pqi.yfazqb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jcm.sufxvd.cn

[R11] case 多分支
来源：http://tod.gotoacloud.top

case "$1" in
来源：http://eal.jlsjyb.cn

start) echo "启动" ;;
来源：http://vkq.nwbrower.top

stop)  echo "停止" ;;
来源：http://eon.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://ufb.shzxlz.cn

esac
来源：http://dbt.cheryme.top

[R12] for 遍历文件
来源：http://qme.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://nlx.jianghu66.top

[R13] for 计数循环
来源：http://fma.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://tmh.ehwqpu.com

[R14] C 风格 for
来源：http://xle.c1oappe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lpe.hysaishi.cn

[R15] while 逐行读文件
来源：http://xuq.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xib.316326.xyz

[R16] until 等待条件
来源：http://ntv.feifeiyinyue.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hgr.ywan-chungtsiang.top

[R17] 数组定义与取值
来源：http://lzy.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://izh.gaohongyu789.top

[R18] 遍历数组
来源：http://uyq.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jzs.zhengqikj.top

[R19] 数组长度
来源：http://oar.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://bfj.xingfuxueyuan.xyz

[R20] 关联数组（字典）
来源：http://ywb.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://slm.havefunace.top

[R21] 字符串长度
来源：http://zpk.pengpengdd.cyou

echo "${#s}"
来源：http://ffl.jqgfzy.top

[R22] 截取子串
来源：http://cma.shzxlz.cn

echo "${s:0:5}"
来源：http://rmy.gotoacloud.top

[R23] 字符串替换
来源：http://inp.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wcg.jinqigfzy.top

[R24] 大小写转换
来源：http://xza.shangyingyoupin.top

echo "${s^^}"; echo "${s,,}"
来源：http://sqm.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://zgr.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qsj.fktsv.cn

[R26] 命令替换
来源：http://rpk.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://mou.bjfxy.top

[R27] 算术展开
来源：http://fpb.jianghu66.top

echo $((1 + 2 * 3))
来源：http://flp.hammf.cn

[R28] 浮点运算
来源：http://xzx.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://ooa.nanxuanxn.top

[R29] 定义函数
来源：http://hnd.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://duf.xinyue.icu

[R30] 函数返回状态码
来源：http://yis.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://mcx.tarul.cn

[R31] 局部变量
来源：http://ouo.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://von.nanxinkj.top

[R32] 参数个数校验
来源：http://kyb.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vdw.yueranfly.top

[R33] 捕获错误并提示行号
来源：http://jlv.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://atl.gzhubu.top

[R34] 退出时清理
来源：http://dpw.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://dvk.fanxiaobao.xyz

[R35] 后台执行并等待
来源：http://jqw.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://gqy.cdnleiting.top

[R36] 并发执行多个任务
来源：http://tvy.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jko.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://dge.cheryme.top

files=$(ls -1)
来源：http://uoj.kuanghao11.cn

[R38] 管道串联
来源：http://tfo.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://pvk.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://kpe.gaohongyu789.top

cmd > out.log 2>&1
来源：http://ofr.jqgfzy.top

[R40] 追加写日志
来源：http://lcy.ctjpmb.com

echo "log" >> out.log
来源：http://ukk.zhoulong.xyz

[R41] 丢弃输出
来源：http://jtw.daria6918.cn

cmd >/dev/null 2>&1
来源：http://dbq.ybcxt.top

[R42] 输入重定向
来源：http://bbj.zhixingplan.top

wc -l < a.txt
来源：http://szd.cqqwz.cn

[R43] 按名字查找文件
来源：http://ess.hcnkem.com

find . -name "*.log" -type f
来源：http://tyh.ctjpmb.com

[R44] 按修改时间查找
来源：http://oug.yvedp.cn

find . -mtime -7 -type f
来源：http://obp.jiagoushi.top

[R45] 批量删除
来源：http://txs.ywan-chungtsiang.top

find . -name "*.tmp" -delete
来源：http://ofe.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://zul.jqgufenzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gph.jinqigufen.top

[R47] sed 单行替换
来源：http://uyq.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://laq.daria6918.cn

[R48] awk 取指定列
来源：http://hfl.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://gbf.hcnkem.com

[R49] awk 带条件
来源：http://hhr.yj20258888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cfn.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://bza.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ydr.ehwqpu.com

[R51] 排序去重取前几
来源：http://zxt.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jha.yonumen.top

[R52] 统计行数
来源：http://edx.jiagoushi.top

wc -l a.txt
来源：http://cat.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://yxb.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lac.birdmap.top

[R54] 比较两个文件
来源：http://shk.xziqi.cn

diff a.txt b.txt
来源：http://guv.sweek.top

[R55] 压缩与解压
来源：http://djb.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mly.wangdashe.top

[R56] 远程拷贝
来源：http://czd.ybcxt.top

scp file user@host:/path/
来源：http://hjs.pengpengdd.cyou

[R57] 远程执行命令
来源：http://ekn.aizwys.cn

ssh user@host 'uptime'
来源：http://sas.sweek.top

[R58] 下载文件
来源：http://xdo.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hab.yfazqb.com

[R59] 发 POST JSON
来源：http://mom.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ybp.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://zgs.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bpu.bjfxy.top

[R61] 磁盘占用
来源：http://sms.andypj.xyz

df -h;  du -sh *
来源：http://tfb.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://oif.zhiwuduotai.top

du -ah . | sort -rh | head -10
来源：http://qdm.hesvh.cn

[R63] 内存与进程
来源：http://nfa.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://oox.zhixingplan.top

[R64] 结束进程
来源：http://oep.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://yuz.guowangkeji.top

[R65] 查看端口占用
来源：http://clt.bjfxy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bxd.tarul.cn

[R66] 定时任务
来源：http://zet.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://zzv.mhx1999.top

[R67] 生成随机十六进制串
来源：http://cfp.vqdsnc.cn

openssl rand -hex 16
来源：http://pdd.nanxuanxn.top

[R68] 计算文件校验值
来源：http://umy.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://sef.zhixingplan.top

[R69] 生成随机密码
来源：http://krh.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://qst.yongpay.top

[R70] 时间戳与互转
来源：http://txh.jyoumei.cn

date +%s;  date -d @1700000000
来源：http://wls.vqdsnc.cn

[R71] 日期格式化
来源：http://gap.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://adw.fengsongda.top

[R72] 等待端口就绪
来源：http://bqg.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dzm.yj20258.top

[R73] 分割大日志
来源：http://nhc.316326.xyz

split -l 1000 big.log part_
来源：http://plv.snrcjt.cn

[R74] 批量重命名
来源：http://yek.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qeb.zdqjudy.top

[R75] 导出环境变量
来源：http://fdy.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://ear.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://jyq.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zxa.jlsjyb.cn

[R77] 读取用户输入
来源：http://pur.zhijiandao.cn

read -rp "请输入: " ans
来源：http://teg.jiagoushi.top

[R78] 交互式菜单
来源：http://vrw.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://ave.yuanzhike.top

[R79] 解析命令行选项
来源：http://auz.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fju.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://yds.0kj1m.cn

time ./run.sh
来源：http://vmo.yj20258.top

================================================================================
来源：http://huy.zycfv.cn

S. C / C++ 专题
来源：http://zyh.kuanghao11.cn

================================================================================
来源：http://vgd.hesvh.cn

[S01] C：Hello World
来源：http://ypt.cqqwz.cn

#include <stdio.h>
来源：http://hol.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ymy.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://vve.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://sfj.0kj1m.cn

[S03] C：读入整数
来源：http://qpa.epnwcf.com

int x; scanf("%d", &x);
来源：http://yzq.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://wqb.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://ueq.daria6918.cn

[S05] C：字符串长度
来源：http://acu.redwolf501.top

strlen(s)
来源：http://bsb.andypj.xyz

[S06] C：字符串比较
来源：http://xux.vehdjk.com

strcmp(a, b) == 0
来源：http://igl.redwolf501.top

[S07] C：数组遍历求和
来源：http://azu.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wlb.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://ajt.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ogg.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://slr.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ply.birdmap.top

[S10] C：指针与解引用
来源：http://bgs.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://uxw.ivvv.top

[S11] C：逐行读文件
来源：http://ebp.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://ajv.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ndo.ywan-chungtsiang.top

fclose(f);
来源：http://ayy.gaohongyu789.top

[S12] C：写文件
来源：http://iff.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ocw.zhoulong.xyz

[S13] C：宏定义
来源：http://jzs.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zxr.yj20258.top

[S14] C：枚举
来源：http://gzi.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://ecu.xylfe.cn

[S15] C：类型转换
来源：http://qyx.tarul.cn

(double) a / b
来源：http://ilj.gotoacloud.top

[S16] C：位操作置位
来源：http://ccr.kuanghao11.cn

x |= (1 << 3);
来源：http://obi.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://ayi.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cmp.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://rdw.zhengqikj.top

int main(int argc, char **argv)
来源：http://euj.fengsongda.top

[S19] C：快速排序
来源：http://avt.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://dvr.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://rgp.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cdf.zhongyouzk.top

[S21] C：字符类别判断
来源：http://hra.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vfg.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://nzz.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://ceu.pycfn.com

[S23] C：随机数
来源：http://mdv.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ryg.shuidangran.top

[S24] C：获取本地时间
来源：http://wac.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xdf.xinyue.icu

[S25] C：内存拷贝
来源：http://nta.shuidangran.top

memcpy(dst, src, n);
来源：http://qtv.vqdsnc.cn

[S26] C：内存清零
来源：http://uyr.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://aqb.tianlin.xyz

[S27] C：定义常量
来源：http://spz.zdbjq.cn

const double PI = 3.14159;
来源：http://ezl.zycfv.cn

[S28] C：静态变量
来源：http://ajo.ehwqpu.com

static int counter = 0;
来源：http://bjg.tianlin.xyz

[S29] C：变参函数
来源：http://pbo.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zvj.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://lmb.zhijiandao.cn

#ifndef X_H
来源：http://qaf.gaohongyu789.top

#define X_H
来源：http://are.yj20258.top

#endif
来源：http://fpa.ctjpmb.com

[S31] C++：Hello World
来源：http://sxw.shangyingyoupin.top

#include <iostream>
来源：http://ibz.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://yvw.aizwys.cn

[S32] C++：字符串
来源：http://myv.yj20258888.top

std::string s = "hi";  s += "!";
来源：http://oke.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://slx.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ect.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://znl.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ccy.uphjek.com

[S35] C++：map
来源：http://ahc.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pzc.gaohongyu789.top

[S36] C++：unordered_map
来源：http://tjx.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lrg.fzhhl.top

[S37] C++：set
来源：http://uuj.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iuq.jqgfzy.top

[S38] C++：排序
来源：http://jch.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://zlc.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://tai.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tsj.feifeiyinyue.top

[S40] C++：查找元素
来源：http://frs.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zpn.daxiang520.top

[S41] C++：类与构造函数
来源：http://ctr.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gal.aizwys.cn

[S42] C++：继承与虚函数
来源：http://idm.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://lvh.hywenlv.cn

[S43] C++：智能指针
来源：http://qmu.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://opm.gotoacloud.top

[S44] C++：引用传参
来源：http://zoo.iojbl.cn

void inc(int &x) { ++x; }
来源：http://feu.wangshuangyany.cn

[S45] C++：lambda
来源：http://ayq.daxiang520.top

auto add = [](int a, int b) { return a + b; };
来源：http://jrx.hammf.cn

[S46] C++：函数模板
来源：http://ory.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eer.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://wnv.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ssp.yongpay.top

[S48] C++：逐行读文件
来源：http://zzn.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://nzt.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://qae.yongpay.top

[S49] C++：写文件
来源：http://leg.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kiv.nwbrower.top

[S50] C++：格式化数字
来源：http://atm.yj20258.top


<!-- 参考信息 -->