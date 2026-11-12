代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wib.fzhhl.top

[Q58] 累计求和
来源：http://voe.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dif.sysykeji.top

[Q59] 分组内累计
来源：http://rml.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dwz.c1oappe.top

[Q60] 取上一行 / 下一行
来源：http://adg.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jfw.pycfn.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hbv.ehwqpu.com

[Q61] 移动平均
来源：http://hez.zhengqikj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://scb.redwolf501.top

[Q62] 分组占比
来源：http://rlj.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pvc.fengsongda.top

[Q63] 开启事务
来源：http://pqc.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://usm.meibo888.top

[Q64] 提交事务
来源：http://bzi.316326.xyz

COMMIT;
来源：http://bwv.zhoulong.xyz

[Q65] 回滚事务
来源：http://ccs.jyoumei.cn

ROLLBACK;
来源：http://umc.fengsongda.top

[Q66] 行锁查询
来源：http://yqz.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vvc.uphjek.com

[Q67] 设置隔离级别
来源：http://ohk.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://skh.ywan-chungtsiang.top

[Q68] 保存点
来源：http://zzt.vqdsnc.cn

SAVEPOINT sp1;
来源：http://tpc.ctjpmb.com

ROLLBACK TO sp1;
来源：http://wnl.dashuyun.cn

[Q69] 查看执行计划
来源：http://lwi.yuxming.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xzn.nanxinkj.top

[Q70] 更新统计信息
来源：http://dje.quarkkingdee.top

ANALYZE TABLE users;
来源：http://fdg.yvedp.cn

[Q71] 查看建表语句
来源：http://dak.shanyushiyangtech.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hje.yj202588.top

[Q72] 查看索引
来源：http://hph.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://xjy.ehwqpu.com

[Q73] 查看表状态
来源：http://rmg.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://dns.kuanghao11.cn

[Q74] 强制使用索引
来源：http://zsd.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hsi.mhx1999.top

[Q75] 日期格式化
来源：http://hpj.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mru.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cqc.svipenyu.cn

[Q76] 按天统计
来源：http://jwd.zdqjudy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dos.ybcxt.top

[Q77] 时间加减
来源：http://nxs.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ioh.sysykeji.top

[Q78] 当前时间
来源：http://qcz.sjlbkw.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hei.jlsjyb.cn

[Q79] 字符串拼接
来源：http://cqn.gzhubu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ccv.epnwcf.com

[Q80] 字符串截取
来源：http://qjb.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dnb.hywenlv.cn

[Q81] 字符串替换
来源：http://fxi.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uqi.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://ayr.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ath.jinqigufen.top

[Q83] 大小写转换
来源：http://ozx.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://egd.cheryme.top

[Q84] 去除首尾空格
来源：http://yet.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://pov.nanxuanxn.top

[Q85] 数值取整
来源：http://rll.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zpj.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://ysq.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lhs.fktsv.cn

[Q87] JSON 字段做条件
来源：http://bwg.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://twd.wangdashe.top

[Q88] 行转列（条件聚合）
来源：http://bpg.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xsm.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pry.tarul.cn

[Q89] 判断表是否存在
来源：http://bae.shanyushiyangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://loi.zdqjudy.top

[Q90] 生成序号列
来源：http://kib.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xhz.tarul.cn

================================================================================
来源：http://vhb.jqgfzy.top

R. Bash 专题
来源：http://imd.redwolf501.top

================================================================================
来源：http://fgs.bbcook.cn

[R01] shebang 与严格模式
来源：http://coi.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://hli.yfazqb.com

set -euo pipefail
来源：http://nek.tian-w.cn

[R02] 变量赋值与使用
来源：http://nzd.yfazqb.com

name="Tom"; echo "$name"
来源：http://jut.svipenyu.cn

[R03] 只读变量
来源：http://wsg.52xcode.cn

readonly PI=3.14
来源：http://jqz.jqgfzy.top

[R04] 位置参数
来源：http://oti.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cvr.jlsjyb.cn

[R05] 参数默认值
来源：http://itn.svipenyu.cn

name="${1:-default}"
来源：http://buz.xuetiantiany.cn

[R06] 判断命令是否存在
来源：http://mrd.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jlv.gaohongyu789.top

[R07] if 判断文件
来源：http://yec.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qie.xylfe.cn

[R08] 数值比较
来源：http://jsq.gaohongyu789.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jqe.jlsjyb.cn

[R09] 字符串比较
来源：http://rub.jinqigufen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gvs.bbcook.cn

[R10] 正则匹配
来源：http://fko.fktsv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xxa.c1oappe.top

[R11] case 多分支
来源：http://vma.mhx1999.top

case "$1" in
来源：http://ahx.shzxlz.cn

start) echo "启动" ;;
来源：http://xbh.jinqigufen.top

stop)  echo "停止" ;;
来源：http://cfs.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://ouc.daria6918.cn

esac
来源：http://uvk.kuanghao11.cn

[R12] for 遍历文件
来源：http://tqk.shzxlz.cn

for f in *.txt; do echo "$f"; done
来源：http://chc.cashguo.top

[R13] for 计数循环
来源：http://qxq.zhoulong.xyz

for i in {1..10}; do echo "$i"; done
来源：http://kgt.yj202588.top

[R14] C 风格 for
来源：http://wmq.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fbe.hysaishi.cn

[R15] while 逐行读文件
来源：http://ily.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://izy.tanke756.top

[R16] until 等待条件
来源：http://wml.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ysg.ywan-chungtsiang.top

[R17] 数组定义与取值
来源：http://mqa.tarul.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wge.ehwqpu.com

[R18] 遍历数组
来源：http://ape.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xiv.fzhhl.top

[R19] 数组长度
来源：http://qpt.yj20258888.top

echo "${#arr[@]}"
来源：http://czw.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://kgb.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://reo.wangshuangyany.cn

[R21] 字符串长度
来源：http://yyt.wangdashe.top

echo "${#s}"
来源：http://mcw.cucudq.cn

[R22] 截取子串
来源：http://puk.sufxvd.cn

echo "${s:0:5}"
来源：http://wck.sxryk.cn

[R23] 字符串替换
来源：http://uar.sjlbkw.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://znw.yj20258888.top

[R24] 大小写转换
来源：http://kxe.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://ytx.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://cbl.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://tgw.uphjek.com

[R26] 命令替换
来源：http://opo.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://xyb.tian-w.cn

[R27] 算术展开
来源：http://rzc.quarkkingdee.top

echo $((1 + 2 * 3))
来源：http://thh.feifeiyinyue.top

[R28] 浮点运算
来源：http://pvs.bjfxy.top

echo "scale=2; 10/3" | bc
来源：http://bqr.sysykeji.top

[R29] 定义函数
来源：http://pwp.vehdjk.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ghb.yueranfly.top

[R30] 函数返回状态码
来源：http://trw.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://sgb.shanyushiyangtech.top

[R31] 局部变量
来源：http://qgh.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://uxj.yuxming.cn

[R32] 参数个数校验
来源：http://teg.zdbjq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eyx.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://zwt.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://teb.nanxuanxn.top

[R34] 退出时清理
来源：http://uum.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://erw.tian-w.cn

[R35] 后台执行并等待
来源：http://wtp.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xou.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://wlj.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ybn.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://qzm.yanxiufei.cn

files=$(ls -1)
来源：http://oil.cqqwz.cn

[R38] 管道串联
来源：http://dpg.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://fwg.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://bxg.jinqigufen.top

cmd > out.log 2>&1
来源：http://xsq.hesvh.cn

[R40] 追加写日志
来源：http://fvp.yuxming.cn

echo "log" >> out.log
来源：http://kvi.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://zau.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://xzv.meibo888.top

[R42] 输入重定向
来源：http://iuy.shzxlz.cn

wc -l < a.txt
来源：http://qvb.bbcook.cn

[R43] 按名字查找文件
来源：http://gri.cheryme.top

find . -name "*.log" -type f
来源：http://fik.jianghu66.top

[R44] 按修改时间查找
来源：http://xnb.316326.xyz

find . -mtime -7 -type f
来源：http://mkh.fengsongda.top

[R45] 批量删除
来源：http://qdv.tian-w.cn

find . -name "*.tmp" -delete
来源：http://sal.wangdashe.top

[R46] 递归替换文件内容
来源：http://qtd.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vpv.quarkkingdee.top

[R47] sed 单行替换
来源：http://jzc.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jdx.hesvh.cn

[R48] awk 取指定列
来源：http://osn.cheryme.top

awk '{print $1, $3}' a.txt
来源：http://odq.yanxiufei.cn

[R49] awk 带条件
来源：http://gpm.ydjk.org.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lke.cqqwz.cn

[R50] awk 求和
来源：http://pkk.nanxuanxn.top

awk '{s += $2} END {print s}' a.txt
来源：http://vqy.vehdjk.com

[R51] 排序去重取前几
来源：http://vck.shanyushiyangtech.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rto.fktsv.cn

[R52] 统计行数
来源：http://iof.yuxming.cn

wc -l a.txt
来源：http://vzz.tian-w.cn

[R53] 查看文件头与实时尾
来源：http://bax.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uko.xuetiantiany.cn

[R54] 比较两个文件
来源：http://fwf.jiagoushi.top

diff a.txt b.txt
来源：http://byr.yj202588.top

[R55] 压缩与解压
来源：http://xjz.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vul.nanxuanxn.top

[R56] 远程拷贝
来源：http://lgd.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://ely.feifeiyinyue.top

[R57] 远程执行命令
来源：http://cfi.bjfxy.top

ssh user@host 'uptime'
来源：http://sgv.zdbjq.cn

[R58] 下载文件
来源：http://hvv.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bbz.jinqigufen.top

[R59] 发 POST JSON
来源：http://tdi.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://avk.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://npf.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nea.aibaodan.cn

[R61] 磁盘占用
来源：http://bgr.fzhhl.top

df -h;  du -sh *
来源：http://ton.cheryme.top

[R62] 找最占空间的文件
来源：http://dch.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://wsu.tianlin.xyz

[R63] 内存与进程
来源：http://bns.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://tpp.jlsjyb.cn

[R64] 结束进程
来源：http://gqy.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://gal.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://xmf.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zhl.0kj1m.cn

[R66] 定时任务
来源：http://iwn.dianchejie.cn

crontab -e;  crontab -l
来源：http://qqg.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://fxa.xuetiantiany.cn

openssl rand -hex 16
来源：http://iof.gzhubu.top

[R68] 计算文件校验值
来源：http://wjd.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lnw.kuanghao11.cn

[R69] 生成随机密码
来源：http://qvu.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://fcc.sweek.top

[R70] 时间戳与互转
来源：http://bol.jianghu66.top

date +%s;  date -d @1700000000
来源：http://cvg.cdnleiting.top

[R71] 日期格式化
来源：http://iaz.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hbi.fengsongda.top

[R72] 等待端口就绪
来源：http://kyy.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://mtl.sxryk.cn

[R73] 分割大日志
来源：http://xtk.zhiwuduotai.top

split -l 1000 big.log part_
来源：http://agd.gotoacloud.top

[R74] 批量重命名
来源：http://trt.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zrt.jianghu66.top

[R75] 导出环境变量
来源：http://hft.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://lau.tarul.cn

[R76] 使用临时文件
来源：http://nwg.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ewa.jinqigufen.top

[R77] 读取用户输入
来源：http://olg.tianlin.xyz

read -rp "请输入: " ans
来源：http://bni.yonumen.top

[R78] 交互式菜单
来源：http://jmc.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://aof.yvedp.cn

[R79] 解析命令行选项
来源：http://tpw.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yhv.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://rpn.yuanzhike.top

time ./run.sh
来源：http://zmt.yfazqb.com

================================================================================
来源：http://blf.dashuyun.cn

S. C / C++ 专题
来源：http://smg.yuxming.cn

================================================================================
来源：http://sgh.yj20258.top

[S01] C：Hello World
来源：http://qgl.chenlongwang.top

#include <stdio.h>
来源：http://jio.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://bgn.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://acy.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://lev.redwolf501.top

[S03] C：读入整数
来源：http://osh.cheryme.top

int x; scanf("%d", &x);
来源：http://tzt.jiagoushi.top

[S04] C：字符串复制
来源：http://shn.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://jgy.hnqzz.top

[S05] C：字符串长度
来源：http://imk.chenzaomai.com

strlen(s)
来源：http://sov.gaohongyu789.top

[S06] C：字符串比较
来源：http://ejh.cqqwz.cn

strcmp(a, b) == 0
来源：http://vcx.havefunace.top

[S07] C：数组遍历求和
来源：http://cke.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jni.ivvv.top

[S08] C：动态内存分配与释放
来源：http://nkq.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wnt.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://ssr.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://njl.zhoulong.xyz

[S10] C：指针与解引用
来源：http://kkm.cashguo.top

int *p = &a;  *p = 5;
来源：http://uwu.hywenlv.cn

[S11] C：逐行读文件
来源：http://ngc.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://vlr.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nkv.ehwqpu.com

fclose(f);
来源：http://ubo.zhaomingkeji.xyz

[S12] C：写文件
来源：http://omi.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sqc.jqgufenzy.top

[S13] C：宏定义
来源：http://uix.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ucq.snrcjt.cn

[S14] C：枚举
来源：http://zbd.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://uli.hammf.cn

[S15] C：类型转换
来源：http://eai.ydzc1.top

(double) a / b
来源：http://gon.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://bzz.cdnleiting.top

x |= (1 << 3);
来源：http://jfv.ybcxt.top

[S17] C：安全拼接字符串
来源：http://wak.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tbq.yfazqb.com

[S18] C：命令行参数
来源：http://qed.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://ipp.xuetiantiany.cn

[S19] C：快速排序
来源：http://pmh.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://nqj.hnxiangtu.top

[S20] C：二分查找
来源：http://mqi.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://chs.daria6918.cn

[S21] C：字符类别判断
来源：http://ujn.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mpn.xinyue.icu

[S22] C：字符串转数字
来源：http://zim.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://okd.0kj1m.cn

[S23] C：随机数
来源：http://czl.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ptd.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://ycb.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lzs.tian-w.cn

[S25] C：内存拷贝
来源：http://xbw.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://plc.chenjidiqi.icu

[S26] C：内存清零
来源：http://eqb.cashguo.top

memset(a, 0, sizeof a);
来源：http://jnk.jqgfzy.top

[S27] C：定义常量
来源：http://sgo.feifeiyinyue.top

const double PI = 3.14159;
来源：http://blz.yj20258888.top

[S28] C：静态变量
来源：http://ygz.tanke756.top


<!-- 参考信息 -->