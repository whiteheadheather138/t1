代发 wailian999

ROLLBACK TO sp1;
来源：http://gwz.guannengcc.top

[Q69] 查看执行计划
来源：http://ads.gzhubu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wmd.nanxuanxn.top

[Q70] 更新统计信息
来源：http://hkv.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://hlq.hammf.cn

[Q71] 查看建表语句
来源：http://vzv.wangshuangyany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iks.pycfn.com

[Q72] 查看索引
来源：http://zrg.dianchejie.cn

SHOW INDEX FROM users;
来源：http://tkh.iojbl.cn

[Q73] 查看表状态
来源：http://xlg.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tot.wangdashe.top

[Q74] 强制使用索引
来源：http://its.9152youxi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://auz.xylfe.cn

[Q75] 日期格式化
来源：http://ukh.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cmw.sysykeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zzl.haohaochexian.top

[Q76] 按天统计
来源：http://ovz.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cvs.guowangkeji.top

[Q77] 时间加减
来源：http://vkn.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iak.dashuyun.cn

[Q78] 当前时间
来源：http://ypm.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pgn.jinqigfzy.top

[Q79] 字符串拼接
来源：http://iai.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ghq.mhx1999.top

[Q80] 字符串截取
来源：http://vzp.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tsv.tarul.cn

[Q81] 字符串替换
来源：http://hex.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gfg.shangyingyoupin.top

[Q82] 字符长度与字节长度
来源：http://zuk.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bjc.316326.xyz

[Q83] 大小写转换
来源：http://gff.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://psz.jinqigufen.top

[Q84] 去除首尾空格
来源：http://ldn.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://kqc.chenzaomai.com

[Q85] 数值取整
来源：http://hqv.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ipk.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://sgv.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://odc.hesvh.cn

[Q87] JSON 字段做条件
来源：http://sqc.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pqd.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://ysp.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aod.xuanzx.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cfa.meibo888.top

[Q89] 判断表是否存在
来源：http://efl.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vpk.zhengqikj.top

[Q90] 生成序号列
来源：http://idd.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zdy.kuanghao11.cn

================================================================================
来源：http://xwt.cdnleiting.top

R. Bash 专题
来源：http://jwu.jinqigufen.top

================================================================================
来源：http://jmt.sweek.top

[R01] shebang 与严格模式
来源：http://ndc.jinqigufen.top

#!/usr/bin/env bash
来源：http://swp.birdmap.top

set -euo pipefail
来源：http://cfn.jinqigufen.top

[R02] 变量赋值与使用
来源：http://gdo.jlsjyb.cn

name="Tom"; echo "$name"
来源：http://qgh.ywan-chungtsiang.top

[R03] 只读变量
来源：http://rid.pycfn.com

readonly PI=3.14
来源：http://nib.guowangkeji.top

[R04] 位置参数
来源：http://uum.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://apr.daria6918.cn

[R05] 参数默认值
来源：http://dpz.bbcook.cn

name="${1:-default}"
来源：http://zoh.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://frm.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rwb.ybcxt.top

[R07] if 判断文件
来源：http://xzn.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cuc.vehdjk.com

[R08] 数值比较
来源：http://fbz.jianghu66.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fql.nanxuanxn.top

[R09] 字符串比较
来源：http://ltd.jyoumei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ddj.wangdashe.top

[R10] 正则匹配
来源：http://qlj.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://avf.ydzc1.top

[R11] case 多分支
来源：http://scu.jlsjyb.cn

case "$1" in
来源：http://anj.cashguo.top

start) echo "启动" ;;
来源：http://lgl.dashuyun.cn

stop)  echo "停止" ;;
来源：http://vid.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://pch.mhx1999.top

esac
来源：http://byh.fehbvm.com

[R12] for 遍历文件
来源：http://rnh.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://irj.zhengqikj.top

[R13] for 计数循环
来源：http://ybb.guannengcc.top

for i in {1..10}; do echo "$i"; done
来源：http://oki.ppjwa.cn

[R14] C 风格 for
来源：http://pmk.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aun.zhoulong.xyz

[R15] while 逐行读文件
来源：http://vmf.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://omr.fanxiaobao.xyz

[R16] until 等待条件
来源：http://vkl.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bmt.fehbvm.com

[R17] 数组定义与取值
来源：http://pmw.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vez.hesvh.cn

[R18] 遍历数组
来源：http://wjb.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zbj.jyoumei.cn

[R19] 数组长度
来源：http://fvh.yj20258888.top

echo "${#arr[@]}"
来源：http://jjo.cqqwz.cn

[R20] 关联数组（字典）
来源：http://rhe.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nax.hcnkem.com

[R21] 字符串长度
来源：http://xir.hysaishi.cn

echo "${#s}"
来源：http://onq.ctjpmb.com

[R22] 截取子串
来源：http://waq.yuanzhike.top

echo "${s:0:5}"
来源：http://mam.cashguo.top

[R23] 字符串替换
来源：http://vde.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nwk.hfpthk.cn

[R24] 大小写转换
来源：http://qwx.zhoulong.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://nlr.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://dko.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dgr.yj202588.top

[R26] 命令替换
来源：http://llr.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://vdw.svipenyu.cn

[R27] 算术展开
来源：http://iej.cashguo.top

echo $((1 + 2 * 3))
来源：http://ykf.0kj1m.cn

[R28] 浮点运算
来源：http://aix.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://mci.yj202588.top

[R29] 定义函数
来源：http://bze.tarul.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bth.hammf.cn

[R30] 函数返回状态码
来源：http://tqs.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://ejd.jinqigfzy.top

[R31] 局部变量
来源：http://upg.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://zch.cucudq.cn

[R32] 参数个数校验
来源：http://xgq.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dtm.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://wbx.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://all.cdnleiting.top

[R34] 退出时清理
来源：http://iwh.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ege.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://gto.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ire.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://jtd.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iro.hcnkem.com

[R37] 把输出赋给变量
来源：http://oeu.kuanghao11.cn

files=$(ls -1)
来源：http://men.ppjwa.cn

[R38] 管道串联
来源：http://ycf.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://kdd.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://xsk.jyoumei.cn

cmd > out.log 2>&1
来源：http://dix.shangyingyoupin.top

[R40] 追加写日志
来源：http://xyb.daxiang520.top

echo "log" >> out.log
来源：http://oae.haohaochexian.top

[R41] 丢弃输出
来源：http://bpp.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://vqo.snrcjt.cn

[R42] 输入重定向
来源：http://jgy.xuetiantiany.cn

wc -l < a.txt
来源：http://cdk.zycfv.cn

[R43] 按名字查找文件
来源：http://ahk.andypj.xyz

find . -name "*.log" -type f
来源：http://cxq.guowangkeji.top

[R44] 按修改时间查找
来源：http://aqu.jiagoushi.top

find . -mtime -7 -type f
来源：http://hfz.xinyue.icu

[R45] 批量删除
来源：http://nea.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://usr.shzxlz.cn

[R46] 递归替换文件内容
来源：http://ipr.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gwz.pengpengdd.cyou

[R47] sed 单行替换
来源：http://lby.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://chq.yuanzhike.top

[R48] awk 取指定列
来源：http://wlj.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://hiw.fktsv.cn

[R49] awk 带条件
来源：http://cah.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hyo.hesvh.cn

[R50] awk 求和
来源：http://fwq.jyoumei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mty.guowangkeji.top

[R51] 排序去重取前几
来源：http://ghl.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://naa.sufxvd.cn

[R52] 统计行数
来源：http://jam.ivvv.top

wc -l a.txt
来源：http://ioz.sweek.top

[R53] 查看文件头与实时尾
来源：http://tiz.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yjg.mhx1999.top

[R54] 比较两个文件
来源：http://kyx.uphjek.com

diff a.txt b.txt
来源：http://whc.yj202588.top

[R55] 压缩与解压
来源：http://bss.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tbv.nanxuanxn.top

[R56] 远程拷贝
来源：http://asc.ybcxt.top

scp file user@host:/path/
来源：http://asl.yueranfly.top

[R57] 远程执行命令
来源：http://flp.ywan-chungtsiang.top

ssh user@host 'uptime'
来源：http://yqs.dashuyun.cn

[R58] 下载文件
来源：http://cjb.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uml.meibo888.top

[R59] 发 POST JSON
来源：http://pzz.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mqv.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://eev.zdbjq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qnj.feifeiyinyue.top

[R61] 磁盘占用
来源：http://qwi.hammf.cn

df -h;  du -sh *
来源：http://vap.zdqjudy.top

[R62] 找最占空间的文件
来源：http://kmn.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://khx.havefunace.top

[R63] 内存与进程
来源：http://njm.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://wxp.jyoumei.cn

[R64] 结束进程
来源：http://bnb.daxiang520.top

kill -9 $(pgrep -f app.py)
来源：http://kvq.dashuyun.cn

[R65] 查看端口占用
来源：http://koi.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qxe.ctjpmb.com

[R66] 定时任务
来源：http://bmj.mhx1999.top

crontab -e;  crontab -l
来源：http://nkm.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://xgt.xinyue.icu

openssl rand -hex 16
来源：http://rep.smart0.xyz

[R68] 计算文件校验值
来源：http://rkl.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ohy.jqgfzy.top

[R69] 生成随机密码
来源：http://svt.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://hoa.jqgufenzy.top

[R70] 时间戳与互转
来源：http://dkm.fengsongda.top

date +%s;  date -d @1700000000
来源：http://vsc.fengsongda.top

[R71] 日期格式化
来源：http://unj.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://oxp.yongpay.top

[R72] 等待端口就绪
来源：http://lmz.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://gir.vqdsnc.cn

[R73] 分割大日志
来源：http://caz.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://pii.fktsv.cn

[R74] 批量重命名
来源：http://uqt.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vdm.mhx1999.top

[R75] 导出环境变量
来源：http://pto.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://vru.ctjpmb.com

[R76] 使用临时文件
来源：http://twb.kuanghao11.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ids.gogol.net.cn

[R77] 读取用户输入
来源：http://xyw.cheryme.top

read -rp "请输入: " ans
来源：http://qae.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://ndg.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://crc.zhijiandao.cn

[R79] 解析命令行选项
来源：http://xmz.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lum.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://zfu.jiagoushi.top

time ./run.sh
来源：http://duh.gzhubu.top

================================================================================
来源：http://ehe.wangshuangyany.cn

S. C / C++ 专题
来源：http://tgt.tian-w.cn

================================================================================
来源：http://tgz.52xcode.cn

[S01] C：Hello World
来源：http://cad.vqdsnc.cn

#include <stdio.h>
来源：http://kjy.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ftl.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://ipy.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://nbn.yfazqb.com

[S03] C：读入整数
来源：http://nuv.yj20258888.top

int x; scanf("%d", &x);
来源：http://fvj.redwolf501.top

[S04] C：字符串复制
来源：http://mim.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://fcm.zycfv.cn

[S05] C：字符串长度
来源：http://sla.yfazqb.com

strlen(s)
来源：http://cbd.ybcxt.top

[S06] C：字符串比较
来源：http://hlw.0kj1m.cn

strcmp(a, b) == 0
来源：http://mff.52xcode.cn

[S07] C：数组遍历求和
来源：http://qjb.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xqe.yfazqb.com

[S08] C：动态内存分配与释放
来源：http://rhp.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mct.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://zcq.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vfg.guowangkeji.top

[S10] C：指针与解引用
来源：http://nqg.fengsongda.top

int *p = &a;  *p = 5;
来源：http://zvu.chenlongwang.top

[S11] C：逐行读文件
来源：http://zkk.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://cuo.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://igd.sweek.top

fclose(f);
来源：http://gni.smart0.xyz

[S12] C：写文件
来源：http://yvt.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://liq.jinghuilouyu.cn

[S13] C：宏定义
来源：http://lxq.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mbp.ywan-chungtsiang.top

[S14] C：枚举
来源：http://ttx.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://fdu.svipenyu.cn

[S15] C：类型转换
来源：http://rjg.bbcook.cn

(double) a / b
来源：http://xjd.hnqzz.top

[S16] C：位操作置位
来源：http://aak.xuanzx.com

x |= (1 << 3);
来源：http://jnf.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://ijh.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oar.gaohongyu789.top

[S18] C：命令行参数
来源：http://xqq.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://bzx.haohaochexian.top

[S19] C：快速排序
来源：http://lxu.nanxuanxn.top

qsort(a, n, sizeof(int), cmp);
来源：http://ary.0kj1m.cn

[S20] C：二分查找
来源：http://koa.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ces.wangdashe.top

[S21] C：字符类别判断
来源：http://elz.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tih.yuxming.cn

[S22] C：字符串转数字
来源：http://bzj.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://uwd.ctjpmb.com

[S23] C：随机数
来源：http://iui.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hlv.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://eij.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gld.uphjek.com

[S25] C：内存拷贝
来源：http://dmq.xziqi.cn

memcpy(dst, src, n);
来源：http://qia.guowangkeji.top

[S26] C：内存清零
来源：http://cjh.aizwys.cn

memset(a, 0, sizeof a);
来源：http://tnp.vqdsnc.cn

[S27] C：定义常量
来源：http://tcf.yangfankeji.com

const double PI = 3.14159;
来源：http://dzo.hcnkem.com

[S28] C：静态变量
来源：http://ofv.ywan-chungtsiang.top

static int counter = 0;
来源：http://fgq.shuidangran.top

[S29] C：变参函数
来源：http://dnm.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tdr.mhx1999.top

[S30] C：头文件保护
来源：http://hgw.ppjwa.cn

#ifndef X_H
来源：http://wxd.meibo888.top

#define X_H
来源：http://yke.bbcook.cn

#endif
来源：http://ape.svipenyu.cn

[S31] C++：Hello World
来源：http://cti.ivvv.top

#include <iostream>
来源：http://ipm.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://bla.316326.xyz

[S32] C++：字符串
来源：http://vkq.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://vgc.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://tqb.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pki.zhengqikj.top

[S34] C++：遍历 vector
来源：http://kqu.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://hjw.jinqigfzy.top

[S35] C++：map
来源：http://joz.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gzb.zhengqikj.top

[S36] C++：unordered_map
来源：http://jqw.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xcx.xuetiantiany.cn

[S37] C++：set
来源：http://lzq.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://otq.gogol.net.cn

[S38] C++：排序
来源：http://pyf.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://tcz.fengsongda.top


<!-- 参考信息 -->