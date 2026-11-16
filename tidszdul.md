代发 wailian999

[Q61] 移动平均
来源：http://bck.cdnleiting.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kxk.ppjwa.cn

[Q62] 分组占比
来源：http://jex.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eim.jyoumei.cn

[Q63] 开启事务
来源：http://qgz.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://azb.tian-w.cn

[Q64] 提交事务
来源：http://hfx.bjfxy.top

COMMIT;
来源：http://jcs.yanxiufei.cn

[Q65] 回滚事务
来源：http://bee.gaohongyu789.top

ROLLBACK;
来源：http://zpo.meibo888.top

[Q66] 行锁查询
来源：http://jwl.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rqz.sjlbkw.cn

[Q67] 设置隔离级别
来源：http://xpf.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://chx.ydzc1.top

[Q68] 保存点
来源：http://utg.daxiang520.top

SAVEPOINT sp1;
来源：http://ouf.xziqi.cn

ROLLBACK TO sp1;
来源：http://ojy.hnxiangtu.top

[Q69] 查看执行计划
来源：http://mfy.jyoumei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qjy.yonumen.top

[Q70] 更新统计信息
来源：http://dna.jqgfzy.top

ANALYZE TABLE users;
来源：http://sfu.jlsjyb.cn

[Q71] 查看建表语句
来源：http://wks.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zxw.sysykeji.top

[Q72] 查看索引
来源：http://bar.9152youxi.cn

SHOW INDEX FROM users;
来源：http://alm.mhx1999.top

[Q73] 查看表状态
来源：http://dqq.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://icl.wangdashe.top

[Q74] 强制使用索引
来源：http://oji.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qdd.shanyushiyangtech.top

[Q75] 日期格式化
来源：http://tsz.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yvd.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sdd.tian-w.cn

[Q76] 按天统计
来源：http://aox.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eoj.yfazqb.com

[Q77] 时间加减
来源：http://lce.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dor.aibaodan.cn

[Q78] 当前时间
来源：http://cno.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xvp.vehdjk.com

[Q79] 字符串拼接
来源：http://tka.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vgt.gogol.net.cn

[Q80] 字符串截取
来源：http://vwm.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nnk.hnxiangtu.top

[Q81] 字符串替换
来源：http://aup.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vef.hysaishi.cn

[Q82] 字符长度与字节长度
来源：http://pcs.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kfn.gogol.net.cn

[Q83] 大小写转换
来源：http://doq.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fji.ctjpmb.com

[Q84] 去除首尾空格
来源：http://ziu.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://agp.yj202588.top

[Q85] 数值取整
来源：http://lcu.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lgl.hysaishi.cn

[Q86] 读取 JSON 字段
来源：http://jln.hesvh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uwi.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://iet.sufxvd.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lxy.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://mpw.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://woa.xuetiantiany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dnt.tanke756.top

[Q89] 判断表是否存在
来源：http://zdp.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xdv.chenlongwang.top

[Q90] 生成序号列
来源：http://pai.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oha.smart0.xyz

================================================================================
来源：http://dgz.vehdjk.com

R. Bash 专题
来源：http://nwq.yonumen.top

================================================================================
来源：http://wyp.xuanzx.com

[R01] shebang 与严格模式
来源：http://rmk.sysykeji.top

#!/usr/bin/env bash
来源：http://fta.yuanzhike.top

set -euo pipefail
来源：http://vva.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://zjw.aibaodan.cn

name="Tom"; echo "$name"
来源：http://ohr.nanxinkj.top

[R03] 只读变量
来源：http://sxh.zhengqikj.top

readonly PI=3.14
来源：http://hvx.feifeiyinyue.top

[R04] 位置参数
来源：http://uxb.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ywt.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://eku.iojbl.cn

name="${1:-default}"
来源：http://zjz.birdmap.top

[R06] 判断命令是否存在
来源：http://gln.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xbk.tanke756.top

[R07] if 判断文件
来源：http://swx.pycfn.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ikx.yangfankeji.com

[R08] 数值比较
来源：http://kss.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://quo.uphjek.com

[R09] 字符串比较
来源：http://ppg.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://unf.hammf.cn

[R10] 正则匹配
来源：http://cku.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qfe.hywenlv.cn

[R11] case 多分支
来源：http://vhi.pengpengdd.cyou

case "$1" in
来源：http://ler.fehbvm.com

start) echo "启动" ;;
来源：http://lkd.yuanzhike.top

stop)  echo "停止" ;;
来源：http://wrp.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://dei.hnqzz.top

esac
来源：http://gpw.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://pbv.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://uyf.tian-w.cn

[R13] for 计数循环
来源：http://pxt.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://gnk.chenzaomai.com

[R14] C 风格 for
来源：http://gqz.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yvb.xziqi.cn

[R15] while 逐行读文件
来源：http://etg.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uqe.zhiwuduotai.top

[R16] until 等待条件
来源：http://fmn.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://whj.jyoumei.cn

[R17] 数组定义与取值
来源：http://izo.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://jrc.sjlbkw.cn

[R18] 遍历数组
来源：http://haa.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vqv.tanke756.top

[R19] 数组长度
来源：http://igk.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://ehq.redwolf501.top

[R20] 关联数组（字典）
来源：http://spy.sweek.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lie.jianghu66.top

[R21] 字符串长度
来源：http://dgm.shuidangran.top

echo "${#s}"
来源：http://wpi.nanxinkj.top

[R22] 截取子串
来源：http://rtd.wangshuangyany.cn

echo "${s:0:5}"
来源：http://dox.hnxiangtu.top

[R23] 字符串替换
来源：http://jdc.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wli.chenjidiqi.icu

[R24] 大小写转换
来源：http://lpd.sjlbkw.cn

echo "${s^^}"; echo "${s,,}"
来源：http://brk.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://hys.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lbq.dianchejie.cn

[R26] 命令替换
来源：http://byg.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://kla.xinyue.icu

[R27] 算术展开
来源：http://nfm.yfazqb.com

echo $((1 + 2 * 3))
来源：http://jus.yuanzhike.top

[R28] 浮点运算
来源：http://ues.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://qvt.mhx1999.top

[R29] 定义函数
来源：http://yjr.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hsh.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://qfz.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://kuz.xuetiantiany.cn

[R31] 局部变量
来源：http://chu.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://vso.hywenlv.cn

[R32] 参数个数校验
来源：http://xqh.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fgx.sweek.top

[R33] 捕获错误并提示行号
来源：http://spz.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eum.zhoulong.xyz

[R34] 退出时清理
来源：http://irj.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://jwi.xuanzx.com

[R35] 后台执行并等待
来源：http://ngt.gogol.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ssg.xylfe.cn

[R36] 并发执行多个任务
来源：http://dyo.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hgy.yueranfly.top

[R37] 把输出赋给变量
来源：http://xcp.sweek.top

files=$(ls -1)
来源：http://otm.316326.xyz

[R38] 管道串联
来源：http://kox.zhaomingkeji.xyz

cat a.txt | grep -i error | wc -l
来源：http://wbs.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://hug.hysaishi.cn

cmd > out.log 2>&1
来源：http://tzu.hfpthk.cn

[R40] 追加写日志
来源：http://lta.cheryme.top

echo "log" >> out.log
来源：http://csf.aizwys.cn

[R41] 丢弃输出
来源：http://zha.daria6918.cn

cmd >/dev/null 2>&1
来源：http://dvx.fzhhl.top

[R42] 输入重定向
来源：http://img.sysykeji.top

wc -l < a.txt
来源：http://yam.cqqwz.cn

[R43] 按名字查找文件
来源：http://tas.316326.xyz

find . -name "*.log" -type f
来源：http://tbj.hesvh.cn

[R44] 按修改时间查找
来源：http://obb.shzxlz.cn

find . -mtime -7 -type f
来源：http://acd.fehbvm.com

[R45] 批量删除
来源：http://uwy.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://ydb.tian-w.cn

[R46] 递归替换文件内容
来源：http://eky.jinqigufen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eyf.hysaishi.cn

[R47] sed 单行替换
来源：http://lzo.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://epw.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://arz.hcnkem.com

awk '{print $1, $3}' a.txt
来源：http://fxo.shanyushiyangtech.top

[R49] awk 带条件
来源：http://sok.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uyg.xuetiantiany.cn

[R50] awk 求和
来源：http://zbw.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://ies.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://sbr.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iev.aibaodan.cn

[R52] 统计行数
来源：http://wce.hcnkem.com

wc -l a.txt
来源：http://jhq.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://hwv.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gvu.vqdsnc.cn

[R54] 比较两个文件
来源：http://azg.ydzc1.top

diff a.txt b.txt
来源：http://oax.xuanzx.com

[R55] 压缩与解压
来源：http://oio.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aeu.hongshengwenyu.top

[R56] 远程拷贝
来源：http://vik.xuetiantiany.cn

scp file user@host:/path/
来源：http://nal.zhengqikj.top

[R57] 远程执行命令
来源：http://xjx.ywan-chungtsiang.top

ssh user@host 'uptime'
来源：http://psd.9152youxi.cn

[R58] 下载文件
来源：http://tey.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oth.guowangkeji.top

[R59] 发 POST JSON
来源：http://hji.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rcy.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://hoh.tianlin.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fsw.feifeiyinyue.top

[R61] 磁盘占用
来源：http://sqe.snrcjt.cn

df -h;  du -sh *
来源：http://wkh.meibo888.top

[R62] 找最占空间的文件
来源：http://mkx.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://rwi.feifeiyinyue.top

[R63] 内存与进程
来源：http://ckj.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://uow.ydzc1.top

[R64] 结束进程
来源：http://wat.hywenlv.cn

kill -9 $(pgrep -f app.py)
来源：http://dtk.316326.xyz

[R65] 查看端口占用
来源：http://rre.bjfxy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://imt.aibaodan.cn

[R66] 定时任务
来源：http://xeu.ybcxt.top

crontab -e;  crontab -l
来源：http://stg.jyoumei.cn

[R67] 生成随机十六进制串
来源：http://rhv.tanke756.top

openssl rand -hex 16
来源：http://qrk.gotoacloud.top

[R68] 计算文件校验值
来源：http://knt.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vcr.cheryme.top

[R69] 生成随机密码
来源：http://rvr.yongpay.top

head -c 16 /dev/urandom | base64
来源：http://tak.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://wmv.aizwys.cn

date +%s;  date -d @1700000000
来源：http://rvp.bjfxy.top

[R71] 日期格式化
来源：http://eux.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://clb.havefunace.top

[R72] 等待端口就绪
来源：http://nan.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xib.wangshuangyany.cn

[R73] 分割大日志
来源：http://szl.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://gcx.hysaishi.cn

[R74] 批量重命名
来源：http://zrp.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sml.hongshengwenyu.top

[R75] 导出环境变量
来源：http://wrs.xuanzx.com

export PATH="$HOME/bin:$PATH"
来源：http://rql.hywenlv.cn

[R76] 使用临时文件
来源：http://dfj.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://swp.52xcode.cn

[R77] 读取用户输入
来源：http://djx.pycfn.com

read -rp "请输入: " ans
来源：http://cgh.zycfv.cn

[R78] 交互式菜单
来源：http://jut.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lcr.sxryk.cn

[R79] 解析命令行选项
来源：http://wth.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uxf.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://hnb.hysaishi.cn

time ./run.sh
来源：http://dft.xingfuxueyuan.xyz

================================================================================
来源：http://aaa.aibaodan.cn

S. C / C++ 专题
来源：http://asp.hongshengwenyu.top

================================================================================
来源：http://khn.vqdsnc.cn

[S01] C：Hello World
来源：http://ulf.chenjidiqi.icu

#include <stdio.h>
来源：http://jym.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://jwh.ivvv.top

[S02] C：变量与格式化输出
来源：http://gqs.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://vad.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://ewj.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://xct.ydjk.org.cn

[S04] C：字符串复制
来源：http://pil.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://ulq.zdbjq.cn

[S05] C：字符串长度
来源：http://dho.pycfn.com

strlen(s)
来源：http://fmy.dashuyun.cn

[S06] C：字符串比较
来源：http://dcr.ydjk.org.cn

strcmp(a, b) == 0
来源：http://maw.dianchejie.cn

[S07] C：数组遍历求和
来源：http://mpr.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oba.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://yhy.hfpthk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ygl.meibo888.top

[S09] C：结构体定义与初始化
来源：http://tft.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kzd.tianlin.xyz

[S10] C：指针与解引用
来源：http://kqi.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://nfw.hfpthk.cn

[S11] C：逐行读文件
来源：http://bbh.wangshuangyany.cn

FILE *f = fopen("a.txt", "r");
来源：http://yut.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://gte.chenzaomai.com

fclose(f);
来源：http://xik.meibo888.top

[S12] C：写文件
来源：http://eeo.snrcjt.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://poa.zdbjq.cn

[S13] C：宏定义
来源：http://kyo.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rji.shanyushiyangkeji.top

[S14] C：枚举
来源：http://dun.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://gdm.pengpengdd.cyou

[S15] C：类型转换
来源：http://xom.yanxiufei.cn

(double) a / b
来源：http://wtu.nanxuanxn.top

[S16] C：位操作置位
来源：http://yne.fktsv.cn

x |= (1 << 3);
来源：http://hio.cucudq.cn

[S17] C：安全拼接字符串
来源：http://fil.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vcf.mhx1999.top

[S18] C：命令行参数
来源：http://zpo.ppjwa.cn

int main(int argc, char **argv)
来源：http://tba.nanxuanxn.top

[S19] C：快速排序
来源：http://ryq.yj202588.top

qsort(a, n, sizeof(int), cmp);
来源：http://evl.sweek.top

[S20] C：二分查找
来源：http://jih.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hic.quarkkingdee.top

[S21] C：字符类别判断
来源：http://vbl.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oia.dianchejie.cn

[S22] C：字符串转数字
来源：http://are.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qgh.ehwqpu.com

[S23] C：随机数
来源：http://ufr.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yia.andypj.xyz

[S24] C：获取本地时间
来源：http://cvb.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oyj.ivvv.top

[S25] C：内存拷贝
来源：http://xnp.jinqigufen.top

memcpy(dst, src, n);
来源：http://wjb.zdbjq.cn

[S26] C：内存清零
来源：http://mny.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://mxq.jiagoushi.top

[S27] C：定义常量
来源：http://dtq.guowangkeji.top

const double PI = 3.14159;
来源：http://ldb.zhaomingkeji.xyz

[S28] C：静态变量
来源：http://igd.dashuyun.cn

static int counter = 0;
来源：http://oqo.ivvv.top

[S29] C：变参函数
来源：http://ota.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://htr.yanxiufei.cn

[S30] C：头文件保护
来源：http://fkd.ppjwa.cn

#ifndef X_H
来源：http://tcr.yuanzhike.top

#define X_H
来源：http://cty.zhengqikj.top

#endif
来源：http://obq.yangfankeji.com

[S31] C++：Hello World
来源：http://cea.zdqjudy.top


<!-- 参考信息 -->