代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tjc.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://tgu.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jiz.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dyo.hongshengwenyu.top

[Q61] 移动平均
来源：http://etu.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lnk.0kj1m.cn

[Q62] 分组占比
来源：http://skm.daxiang520.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xgi.hnxiangtu.top

[Q63] 开启事务
来源：http://bsh.yanxiufei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://arg.uphjek.com

[Q64] 提交事务
来源：http://zoz.svipenyu.cn

COMMIT;
来源：http://vrp.jqgufenzy.top

[Q65] 回滚事务
来源：http://emo.shanyushiyangtech.top

ROLLBACK;
来源：http://hdb.meibo888.top

[Q66] 行锁查询
来源：http://nwo.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nvw.zhoulong.xyz

[Q67] 设置隔离级别
来源：http://bqt.fehbvm.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eow.wangdashe.top

[Q68] 保存点
来源：http://ybx.chenjidiqi.icu

SAVEPOINT sp1;
来源：http://pdi.sjlbkw.cn

ROLLBACK TO sp1;
来源：http://lde.epnwcf.com

[Q69] 查看执行计划
来源：http://mjd.feifeiyinyue.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://swh.c1oappe.top

[Q70] 更新统计信息
来源：http://hjs.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://dug.jqgfzy.top

[Q71] 查看建表语句
来源：http://nwy.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cqx.zhijiandao.cn

[Q72] 查看索引
来源：http://gca.ywan-chungtsiang.top

SHOW INDEX FROM users;
来源：http://vgs.gzhubu.top

[Q73] 查看表状态
来源：http://rls.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qjy.ctjpmb.com

[Q74] 强制使用索引
来源：http://gxc.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bhp.bbcook.cn

[Q75] 日期格式化
来源：http://kki.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rif.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://che.cdnleiting.top

[Q76] 按天统计
来源：http://edd.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mrl.aizwys.cn

[Q77] 时间加减
来源：http://qnu.fengsongda.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vco.jiagoushi.top

[Q78] 当前时间
来源：http://pwy.ivvv.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fwf.andypj.xyz

[Q79] 字符串拼接
来源：http://tqn.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bzh.hnxiangtu.top

[Q80] 字符串截取
来源：http://bng.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yzk.dashuyun.cn

[Q81] 字符串替换
来源：http://qup.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qgi.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://dgh.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nxa.hysaishi.cn

[Q83] 大小写转换
来源：http://iif.sufxvd.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ofj.hesvh.cn

[Q84] 去除首尾空格
来源：http://huc.52xcode.cn

SELECT TRIM(name) FROM users;
来源：http://rdd.jiagoushi.top

[Q85] 数值取整
来源：http://gls.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bvw.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://tiw.cucudq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iwc.yj20258.top

[Q87] JSON 字段做条件
来源：http://hrx.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hxq.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://wph.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://osy.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hgs.uphjek.com

[Q89] 判断表是否存在
来源：http://wef.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xzd.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://ulw.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://edz.vqdsnc.cn

================================================================================
来源：http://qqf.ctjpmb.com

R. Bash 专题
来源：http://yhc.xuetiantiany.cn

================================================================================
来源：http://oix.fanxiaobao.xyz

[R01] shebang 与严格模式
来源：http://sgi.iojbl.cn

#!/usr/bin/env bash
来源：http://vzu.bjfxy.top

set -euo pipefail
来源：http://xqm.meibo888.top

[R02] 变量赋值与使用
来源：http://nji.guowangkeji.top

name="Tom"; echo "$name"
来源：http://tfr.nanxuanxn.top

[R03] 只读变量
来源：http://nyl.hesvh.cn

readonly PI=3.14
来源：http://wkd.jiagoushi.top

[R04] 位置参数
来源：http://xzi.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fnd.zhiwuduotai.top

[R05] 参数默认值
来源：http://zrh.bjfxy.top

name="${1:-default}"
来源：http://nal.yonumen.top

[R06] 判断命令是否存在
来源：http://lav.wangdashe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://csx.cdnleiting.top

[R07] if 判断文件
来源：http://rfb.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xfe.wangdashe.top

[R08] 数值比较
来源：http://oyq.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tzk.shangyingyoupin.top

[R09] 字符串比较
来源：http://qoq.daxiang520.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mww.guannengcc.top

[R10] 正则匹配
来源：http://gam.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hxu.shanyushiyangkeji.top

[R11] case 多分支
来源：http://nah.zhaomingkeji.xyz

case "$1" in
来源：http://ass.xuanzx.com

start) echo "启动" ;;
来源：http://lqd.fengsongda.top

stop)  echo "停止" ;;
来源：http://lyu.52xcode.cn

*)     echo "未知命令" ;;
来源：http://tpw.zhongyouzk.top

esac
来源：http://erb.daria6918.cn

[R12] for 遍历文件
来源：http://qaz.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://zpr.sufxvd.cn

[R13] for 计数循环
来源：http://rwi.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://qbs.nanxuanxn.top

[R14] C 风格 for
来源：http://ofs.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jce.yvedp.cn

[R15] while 逐行读文件
来源：http://ecm.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ynu.yuanzhike.top

[R16] until 等待条件
来源：http://phz.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gmb.yuanzhike.top

[R17] 数组定义与取值
来源：http://cfg.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://tub.yanxiufei.cn

[R18] 遍历数组
来源：http://elf.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lxz.hfpthk.cn

[R19] 数组长度
来源：http://wmg.hammf.cn

echo "${#arr[@]}"
来源：http://wni.hcnkem.com

[R20] 关联数组（字典）
来源：http://mzn.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nsy.snrcjt.cn

[R21] 字符串长度
来源：http://xyt.52xcode.cn

echo "${#s}"
来源：http://bgn.gotoacloud.top

[R22] 截取子串
来源：http://fnn.nanxuanxn.top

echo "${s:0:5}"
来源：http://lde.yj20258888.top

[R23] 字符串替换
来源：http://pve.xziqi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rwy.sufxvd.cn

[R24] 大小写转换
来源：http://jxk.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://jtl.0kj1m.cn

[R25] 去后缀 / 去前缀
来源：http://kxd.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://myv.jinqigfzy.top

[R26] 命令替换
来源：http://glz.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://bqz.yj202588.top

[R27] 算术展开
来源：http://ouz.smart0.xyz

echo $((1 + 2 * 3))
来源：http://fbe.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://oqv.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://umi.ivvv.top

[R29] 定义函数
来源：http://jhd.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qez.hnxiangtu.top

[R30] 函数返回状态码
来源：http://vzv.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://ygq.fengsongda.top

[R31] 局部变量
来源：http://dsi.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://idt.snrcjt.cn

[R32] 参数个数校验
来源：http://wdp.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://orb.meibo888.top

[R33] 捕获错误并提示行号
来源：http://yay.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dbz.sysykeji.top

[R34] 退出时清理
来源：http://rku.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ygq.yfazqb.com

[R35] 后台执行并等待
来源：http://tci.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xdh.sysykeji.top

[R36] 并发执行多个任务
来源：http://yiv.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zpr.ctjpmb.com

[R37] 把输出赋给变量
来源：http://pxs.zdqjudy.top

files=$(ls -1)
来源：http://ijg.hnxiangtu.top

[R38] 管道串联
来源：http://yhv.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://mzb.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://ati.guannengcc.top

cmd > out.log 2>&1
来源：http://ynz.316326.xyz

[R40] 追加写日志
来源：http://swt.snrcjt.cn

echo "log" >> out.log
来源：http://aos.tian-w.cn

[R41] 丢弃输出
来源：http://zjn.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://dud.dashuyun.cn

[R42] 输入重定向
来源：http://hdb.chenzaomai.com

wc -l < a.txt
来源：http://vph.zdqjudy.top

[R43] 按名字查找文件
来源：http://qhx.ehwqpu.com

find . -name "*.log" -type f
来源：http://wda.cashguo.top

[R44] 按修改时间查找
来源：http://zmg.tian-w.cn

find . -mtime -7 -type f
来源：http://pal.yueranfly.top

[R45] 批量删除
来源：http://ylz.yongpay.top

find . -name "*.tmp" -delete
来源：http://yli.jinqigufen.top

[R46] 递归替换文件内容
来源：http://adz.fktsv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://utw.iojbl.cn

[R47] sed 单行替换
来源：http://stm.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://nkc.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://fbk.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://pji.yongpay.top

[R49] awk 带条件
来源：http://kpm.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://crw.zhijiandao.cn

[R50] awk 求和
来源：http://ptk.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oji.jinqigfzy.top

[R51] 排序去重取前几
来源：http://lbj.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mkv.cheryme.top

[R52] 统计行数
来源：http://eqn.zhongyouzk.top

wc -l a.txt
来源：http://qtc.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://wyg.sxryk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iyl.jinqigufen.top

[R54] 比较两个文件
来源：http://lpu.cucudq.cn

diff a.txt b.txt
来源：http://tmd.jqgfzy.top

[R55] 压缩与解压
来源：http://idd.yfazqb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mzc.jyoumei.cn

[R56] 远程拷贝
来源：http://dya.fzhhl.top

scp file user@host:/path/
来源：http://gdm.chenzaomai.com

[R57] 远程执行命令
来源：http://bam.nwbrower.top

ssh user@host 'uptime'
来源：http://szg.hongshengwenyu.top

[R58] 下载文件
来源：http://vgu.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qqn.gogol.net.cn

[R59] 发 POST JSON
来源：http://phe.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ejp.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://ntu.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kre.sweek.top

[R61] 磁盘占用
来源：http://xub.havefunace.top

df -h;  du -sh *
来源：http://mpk.fehbvm.com

[R62] 找最占空间的文件
来源：http://tcq.bjfxy.top

du -ah . | sort -rh | head -10
来源：http://tdg.hywenlv.cn

[R63] 内存与进程
来源：http://foo.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://hnx.yj20258.top

[R64] 结束进程
来源：http://chg.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://yyb.daria6918.cn

[R65] 查看端口占用
来源：http://tuv.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aak.cqqwz.cn

[R66] 定时任务
来源：http://izk.jqgfzy.top

crontab -e;  crontab -l
来源：http://woi.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://unq.bjfxy.top

openssl rand -hex 16
来源：http://tnr.gogol.net.cn

[R68] 计算文件校验值
来源：http://ekq.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ciz.jyoumei.cn

[R69] 生成随机密码
来源：http://vll.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://bgq.yj202588.top

[R70] 时间戳与互转
来源：http://vvl.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://arw.jinqigfzy.top

[R71] 日期格式化
来源：http://qwr.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bcq.gaohongyu789.top

[R72] 等待端口就绪
来源：http://dad.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mfc.hysaishi.cn

[R73] 分割大日志
来源：http://gwg.smart0.xyz

split -l 1000 big.log part_
来源：http://dns.xuetiantiany.cn

[R74] 批量重命名
来源：http://llr.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ujm.zdqjudy.top

[R75] 导出环境变量
来源：http://ptm.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://syw.xylfe.cn

[R76] 使用临时文件
来源：http://tjx.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qfe.gaohongyu789.top

[R77] 读取用户输入
来源：http://bno.daria6918.cn

read -rp "请输入: " ans
来源：http://yaq.yj20258.top

[R78] 交互式菜单
来源：http://msk.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://xxt.hesvh.cn

[R79] 解析命令行选项
来源：http://wxm.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ijo.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://vfx.tianlin.xyz

time ./run.sh
来源：http://zje.svipenyu.cn

================================================================================
来源：http://pxv.meibo888.top

S. C / C++ 专题
来源：http://eky.svipenyu.cn

================================================================================
来源：http://muk.gaohongyu789.top

[S01] C：Hello World
来源：http://zzo.shanyushiyangkeji.top

#include <stdio.h>
来源：http://gvo.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wsd.yongpay.top

[S02] C：变量与格式化输出
来源：http://mcs.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://lrj.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://ktx.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://khs.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://myz.bjfxy.top

char dst[32]; strcpy(dst, "hi");
来源：http://irt.cheryme.top

[S05] C：字符串长度
来源：http://kkp.yfazqb.com

strlen(s)
来源：http://zjx.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://cbn.yangfankeji.com

strcmp(a, b) == 0
来源：http://ewm.dianchejie.cn

[S07] C：数组遍历求和
来源：http://olz.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sdd.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://dkf.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://njo.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://wxv.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rxv.fengsongda.top

[S10] C：指针与解引用
来源：http://vkq.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://own.sxryk.cn

[S11] C：逐行读文件
来源：http://bvx.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://llq.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kjn.guowangkeji.top

fclose(f);
来源：http://mtq.yonumen.top

[S12] C：写文件
来源：http://ksp.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xyt.ehwqpu.com

[S13] C：宏定义
来源：http://yzg.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://afc.svipenyu.cn

[S14] C：枚举
来源：http://rry.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://twg.yj20258.top

[S15] C：类型转换
来源：http://cfk.gotoacloud.top

(double) a / b
来源：http://niq.iojbl.cn

[S16] C：位操作置位
来源：http://xzj.jiagoushi.top

x |= (1 << 3);
来源：http://gss.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://xwu.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ieg.meibo888.top

[S18] C：命令行参数
来源：http://ztn.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://pdj.hfpthk.cn

[S19] C：快速排序
来源：http://dii.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iyy.guowangkeji.top

[S20] C：二分查找
来源：http://oqm.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://srv.uphjek.com

[S21] C：字符类别判断
来源：http://yoo.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://abl.yj202588.top

[S22] C：字符串转数字
来源：http://ozu.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://fps.quarkkingdee.top

[S23] C：随机数
来源：http://inh.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://phm.zhongyouzk.top

[S24] C：获取本地时间
来源：http://cvi.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eag.ehwqpu.com

[S25] C：内存拷贝
来源：http://ckj.quarkkingdee.top

memcpy(dst, src, n);
来源：http://twa.gzhubu.top

[S26] C：内存清零
来源：http://kpg.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://xiw.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://xcv.yuanzhike.top

const double PI = 3.14159;
来源：http://sga.hysaishi.cn

[S28] C：静态变量
来源：http://ywn.xuanzx.com

static int counter = 0;
来源：http://hdr.cdnleiting.top

[S29] C：变参函数
来源：http://wse.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tpb.sufxvd.cn

[S30] C：头文件保护
来源：http://pmt.zhongyouzk.top


<!-- 参考信息 -->