代发 wailian999

[Q76] 按天统计
来源：http://nnh.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rcx.zhijiandao.cn

[Q77] 时间加减
来源：http://hfy.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hvr.tianlin.xyz

[Q78] 当前时间
来源：http://oyb.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cfj.tian-w.cn

[Q79] 字符串拼接
来源：http://eec.wangdashe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xmg.ehwqpu.com

[Q80] 字符串截取
来源：http://pbv.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oxs.bjfxy.top

[Q81] 字符串替换
来源：http://bmk.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ynp.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://giz.zhaomingkeji.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ark.haohaochexian.top

[Q83] 大小写转换
来源：http://kjy.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nbq.mhx1999.top

[Q84] 去除首尾空格
来源：http://ape.kuanghao11.cn

SELECT TRIM(name) FROM users;
来源：http://ipq.sysykeji.top

[Q85] 数值取整
来源：http://ltu.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nzd.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://qxg.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zee.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://iia.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pes.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://ejb.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bcp.vqdsnc.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tlu.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://nhv.zdqjudy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bft.sweek.top

[Q90] 生成序号列
来源：http://pvt.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kzx.ehwqpu.com

================================================================================
来源：http://vtl.gogol.net.cn

R. Bash 专题
来源：http://utx.nwbrower.top

================================================================================
来源：http://jyv.pycfn.com

[R01] shebang 与严格模式
来源：http://kps.jlsjyb.cn

#!/usr/bin/env bash
来源：http://mvk.yonumen.top

set -euo pipefail
来源：http://yss.chenlongwang.top

[R02] 变量赋值与使用
来源：http://fgv.cashguo.top

name="Tom"; echo "$name"
来源：http://phz.tianlin.xyz

[R03] 只读变量
来源：http://wiu.dashuyun.cn

readonly PI=3.14
来源：http://wsb.shanyushiyangtech.top

[R04] 位置参数
来源：http://uhf.9152youxi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bdn.aizwys.cn

[R05] 参数默认值
来源：http://hpg.hesvh.cn

name="${1:-default}"
来源：http://bpf.cdnleiting.top

[R06] 判断命令是否存在
来源：http://wls.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://srk.xinyue.icu

[R07] if 判断文件
来源：http://ola.andypj.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dyu.jiagoushi.top

[R08] 数值比较
来源：http://fuf.yfazqb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://hnf.cucudq.cn

[R09] 字符串比较
来源：http://jfv.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sqt.zhengqikj.top

[R10] 正则匹配
来源：http://ygt.hesvh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lqg.yuanzhike.top

[R11] case 多分支
来源：http://con.ybcxt.top

case "$1" in
来源：http://hoi.shuidangran.top

start) echo "启动" ;;
来源：http://ely.daria6918.cn

stop)  echo "停止" ;;
来源：http://ugo.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://wws.aizwys.cn

esac
来源：http://fta.guowangkeji.top

[R12] for 遍历文件
来源：http://soz.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://sba.ivvv.top

[R13] for 计数循环
来源：http://iyt.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://dts.0kj1m.cn

[R14] C 风格 for
来源：http://tmc.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uft.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://byn.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hzf.hcnkem.com

[R16] until 等待条件
来源：http://roj.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mue.vqdsnc.cn

[R17] 数组定义与取值
来源：http://rql.daria6918.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oay.yj202588.top

[R18] 遍历数组
来源：http://qvb.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cml.yj202588.top

[R19] 数组长度
来源：http://ckv.sjlbkw.cn

echo "${#arr[@]}"
来源：http://mkn.iojbl.cn

[R20] 关联数组（字典）
来源：http://gaq.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://haf.tianlin.xyz

[R21] 字符串长度
来源：http://lca.hnqzz.top

echo "${#s}"
来源：http://rtl.andypj.xyz

[R22] 截取子串
来源：http://orl.shuidangran.top

echo "${s:0:5}"
来源：http://nvi.nanxuanxn.top

[R23] 字符串替换
来源：http://wfb.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://avd.52xcode.cn

[R24] 大小写转换
来源：http://zey.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://mym.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://xce.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://hbh.yonumen.top

[R26] 命令替换
来源：http://zan.yj202588.top

now=$(date +%F); echo "$now"
来源：http://vvg.yuanzhike.top

[R27] 算术展开
来源：http://kfw.uphjek.com

echo $((1 + 2 * 3))
来源：http://czt.birdmap.top

[R28] 浮点运算
来源：http://qds.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://yre.jlsjyb.cn

[R29] 定义函数
来源：http://kky.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fdl.daria6918.cn

[R30] 函数返回状态码
来源：http://ehj.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://maj.bjfxy.top

[R31] 局部变量
来源：http://xfu.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://hcs.sxryk.cn

[R32] 参数个数校验
来源：http://dep.birdmap.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dcv.yj202588.top

[R33] 捕获错误并提示行号
来源：http://lid.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dzu.yuanzhike.top

[R34] 退出时清理
来源：http://swn.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://fbv.sxryk.cn

[R35] 后台执行并等待
来源：http://bzh.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ors.cucudq.cn

[R36] 并发执行多个任务
来源：http://npx.ppjwa.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oqs.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://oac.sxryk.cn

files=$(ls -1)
来源：http://xdo.xylfe.cn

[R38] 管道串联
来源：http://fme.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://zqd.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://qog.tian-w.cn

cmd > out.log 2>&1
来源：http://tdx.kuanghao11.cn

[R40] 追加写日志
来源：http://amc.yj202588.top

echo "log" >> out.log
来源：http://ltt.yonumen.top

[R41] 丢弃输出
来源：http://rve.aizwys.cn

cmd >/dev/null 2>&1
来源：http://opw.ppjwa.cn

[R42] 输入重定向
来源：http://eto.316326.xyz

wc -l < a.txt
来源：http://tnu.hcnkem.com

[R43] 按名字查找文件
来源：http://hoo.ctjpmb.com

find . -name "*.log" -type f
来源：http://syk.xuanzx.com

[R44] 按修改时间查找
来源：http://gtn.gotoacloud.top

find . -mtime -7 -type f
来源：http://zad.guannengcc.top

[R45] 批量删除
来源：http://tja.andypj.xyz

find . -name "*.tmp" -delete
来源：http://eri.zhengqikj.top

[R46] 递归替换文件内容
来源：http://rgu.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://olu.zhongyouzk.top

[R47] sed 单行替换
来源：http://gjf.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://ksz.yangfankeji.com

[R48] awk 取指定列
来源：http://fwi.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://vvk.cqqwz.cn

[R49] awk 带条件
来源：http://frn.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pat.ydjk.org.cn

[R50] awk 求和
来源：http://bvm.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jwd.guowangkeji.top

[R51] 排序去重取前几
来源：http://uov.fengsongda.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ixd.hesvh.cn

[R52] 统计行数
来源：http://tqe.0kj1m.cn

wc -l a.txt
来源：http://qnk.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://ztq.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rqs.jqgfzy.top

[R54] 比较两个文件
来源：http://gfh.zhaomingkeji.xyz

diff a.txt b.txt
来源：http://tpy.aibaodan.cn

[R55] 压缩与解压
来源：http://csz.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dcj.sweek.top

[R56] 远程拷贝
来源：http://gar.xuanzx.com

scp file user@host:/path/
来源：http://kav.cucudq.cn

[R57] 远程执行命令
来源：http://cbk.ctjpmb.com

ssh user@host 'uptime'
来源：http://clg.jqgufenzy.top

[R58] 下载文件
来源：http://kve.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tyv.zdqjudy.top

[R59] 发 POST JSON
来源：http://fuw.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wmm.zdbjq.cn

[R60] 只看 HTTP 状态码
来源：http://xbf.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zzz.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://cos.nanxuanxn.top

df -h;  du -sh *
来源：http://baj.nanxinkj.top

[R62] 找最占空间的文件
来源：http://guc.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://swy.cqqwz.cn

[R63] 内存与进程
来源：http://cne.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://rdy.hongshengwenyu.top

[R64] 结束进程
来源：http://lsr.meibo888.top

kill -9 $(pgrep -f app.py)
来源：http://gjo.aizwys.cn

[R65] 查看端口占用
来源：http://lgz.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qmy.gogol.net.cn

[R66] 定时任务
来源：http://zpg.ppjwa.cn

crontab -e;  crontab -l
来源：http://nlx.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://jqk.ehwqpu.com

openssl rand -hex 16
来源：http://cpv.dashuyun.cn

[R68] 计算文件校验值
来源：http://lff.andypj.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://fim.daxiang520.top

[R69] 生成随机密码
来源：http://xfi.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://qmm.bjfxy.top

[R70] 时间戳与互转
来源：http://ihz.xuanzx.com

date +%s;  date -d @1700000000
来源：http://kok.wangshuangyany.cn

[R71] 日期格式化
来源：http://woy.jinqigfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lhq.hammf.cn

[R72] 等待端口就绪
来源：http://vnx.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qjk.yj20258888.top

[R73] 分割大日志
来源：http://mod.sysykeji.top

split -l 1000 big.log part_
来源：http://igh.ydjk.org.cn

[R74] 批量重命名
来源：http://ecc.jiagoushi.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iui.pycfn.com

[R75] 导出环境变量
来源：http://rad.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://gij.yonumen.top

[R76] 使用临时文件
来源：http://kox.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lfp.zdqjudy.top

[R77] 读取用户输入
来源：http://nxe.yangfankeji.com

read -rp "请输入: " ans
来源：http://sbc.mhx1999.top

[R78] 交互式菜单
来源：http://faq.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gsu.tian-w.cn

[R79] 解析命令行选项
来源：http://qke.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ngk.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://fas.nanxinkj.top

time ./run.sh
来源：http://hrz.cheryme.top

================================================================================
来源：http://ozp.hesvh.cn

S. C / C++ 专题
来源：http://wmg.zhiwuduotai.top

================================================================================
来源：http://abj.zdqjudy.top

[S01] C：Hello World
来源：http://nmo.cucudq.cn

#include <stdio.h>
来源：http://kjp.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ytm.meibo888.top

[S02] C：变量与格式化输出
来源：http://kjc.yanxiufei.cn

int a = 10; printf("%d\n", a);
来源：http://bda.shanyushiyangtech.top

[S03] C：读入整数
来源：http://drf.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://qpq.tian-w.cn

[S04] C：字符串复制
来源：http://ikq.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://bef.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://ajq.tarul.cn

strlen(s)
来源：http://bam.quarkkingdee.top

[S06] C：字符串比较
来源：http://vnj.yj20258888.top

strcmp(a, b) == 0
来源：http://trs.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://suj.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vqi.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://rnz.jinyuanbaomall.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xqu.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://lwx.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wmh.xylfe.cn

[S10] C：指针与解引用
来源：http://kxq.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://lpn.uphjek.com

[S11] C：逐行读文件
来源：http://qxu.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://tcg.uphjek.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://zfs.svipenyu.cn

fclose(f);
来源：http://kjy.xuetiantiany.cn

[S12] C：写文件
来源：http://fza.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://skw.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://nfc.52xcode.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://scw.vqdsnc.cn

[S14] C：枚举
来源：http://vtf.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://gii.yvedp.cn

[S15] C：类型转换
来源：http://iuv.gzhubu.top

(double) a / b
来源：http://hom.yj20258.top

[S16] C：位操作置位
来源：http://fek.tian-w.cn

x |= (1 << 3);
来源：http://tlb.yj20258.top

[S17] C：安全拼接字符串
来源：http://cbf.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mkb.sjlbkw.cn

[S18] C：命令行参数
来源：http://int.kuanghao11.cn

int main(int argc, char **argv)
来源：http://ipf.daria6918.cn

[S19] C：快速排序
来源：http://mds.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ftt.jyoumei.cn

[S20] C：二分查找
来源：http://kyu.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nfn.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://uvr.yvedp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tra.zhixingplan.top

[S22] C：字符串转数字
来源：http://fzc.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://ctp.vehdjk.com

[S23] C：随机数
来源：http://riq.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://evn.cqqwz.cn

[S24] C：获取本地时间
来源：http://egd.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dim.sufxvd.cn

[S25] C：内存拷贝
来源：http://uma.gogol.net.cn

memcpy(dst, src, n);
来源：http://kgx.sjlbkw.cn

[S26] C：内存清零
来源：http://bce.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://ibc.yj20258.top

[S27] C：定义常量
来源：http://edt.0kj1m.cn

const double PI = 3.14159;
来源：http://zyv.yonumen.top

[S28] C：静态变量
来源：http://eoa.fengsongda.top

static int counter = 0;
来源：http://cva.nanxinkj.top

[S29] C：变参函数
来源：http://muv.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jso.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://kuz.andypj.xyz

#ifndef X_H
来源：http://uch.sxryk.cn

#define X_H
来源：http://aup.fktsv.cn

#endif
来源：http://ynj.tianlin.xyz

[S31] C++：Hello World
来源：http://rui.pengpengdd.cyou

#include <iostream>
来源：http://fch.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://cpu.chenjidiqi.icu

[S32] C++：字符串
来源：http://daz.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://iqv.zycfv.cn

[S33] C++：vector 增删
来源：http://wdy.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rqi.sjlbkw.cn

[S34] C++：遍历 vector
来源：http://kar.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://nqb.pengpengdd.cyou

[S35] C++：map
来源：http://fkq.jqgufenzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xvq.haohaochexian.top

[S36] C++：unordered_map
来源：http://esd.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nag.yonumen.top

[S37] C++：set
来源：http://yrm.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hod.hcnkem.com

[S38] C++：排序
来源：http://uwz.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://egb.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://hvy.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kcb.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://zle.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qpk.sjlbkw.cn

[S41] C++：类与构造函数
来源：http://bev.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rex.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://gzu.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://lcs.hnqzz.top

[S43] C++：智能指针
来源：http://ajh.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://icj.yueranfly.top

[S44] C++：引用传参
来源：http://lpn.tian-w.cn

void inc(int &x) { ++x; }
来源：http://ewc.sjlbkw.cn

[S45] C++：lambda
来源：http://xil.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://nhd.jinghuilouyu.cn

[S46] C++：函数模板
来源：http://fsh.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tsa.bbcook.cn


<!-- 参考信息 -->